# Je build mon image Dolibarr
#######################
docker build -t dolibarr .

# Je run mon docker Dolibarr
#######################
docker run -it -d --name doli -p80:80 dolibarr:latest 

# Je tag mon build pour le push dans le registry docker hub
#############################################
 docker build -t devopsup/dolibarr:faurecia .

# je me connecte à mon registry
#########################
docker login --username=devopsup

# Je push mon image sur le registry
###########################
docker push devopsup/dolibarr:faurecia

