# Dolibarr + MariaDB

- Build de l'image Dolibarr :
docker build -t dolibarr .

- Run de l'image docker Dolibarr :
docker run -it -d --name doli -p80:80 dolibarr:latest 

- Le tag avant le push dans le registry docker hub :
docker build -t devopsup/dolibarr:faurecia .

- la connexion au registry :
docker login --username=devopsup

- le push dans registry : 
docker push devopsup/dolibarr:faurecia

