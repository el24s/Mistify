# Documentation de l'application web Mistify
Le projet consiste à une application web d'achat de parfums qui agit comme une encyclopédie de parfum où l'on peut laisser des commentaires et faire des demandes d'ajout de parfums.

Les répertoires sont : https://github.com/yanis26x/Mistify-frontend.git & https://github.com/rym31/Mistify-backend.git

## Configuration Base
Configurer les variables d'environnements dans le fichier .env

### Configuration avec Kubernetes et Docker
Lancer la base de données avec la commande
```
sudo docker compose up -d
sudo docker compose down -> pour fermer les containers
```
Lancer le cluster
```
kubectl apply -f mistify-manifests/mistify-frontend/
kubectl apply -f mistify-manifests/mistify-backend/
```
Arrête le cluster
```
kubectl delete -f mistify-manifests/mistify-frontend/
kubectl delete -f mistify-manifests/mistify-backend/
```
                
### Configuration avec Docker seulement
Lancer les services avec la commande
```
sudo docker compose up -d
sudo docker compose down -> pour fermer les containers
```

## Tester l'application web
Rechercher qu'elle port est exposée avec la commande
```
docker ps
```
Rentre l'adresse ip avec le port exposer pour tester que l'application web est fonctionnelle
ex. http://10.10.0.123:80      
