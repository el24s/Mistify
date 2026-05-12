# Documentation
TODOO -> maybe secret implémentation ou autre pour la value/url pour backend accede a la BD a regarder ici
    - https://kubernetes.io/docs/concepts/configuration/secret/ 

Configuration
- lien vers docker compose BD
    - https://hub.docker.com/_/mongo?xk=ShowRecommendedBadge&xt=Disabled



Étapes
- Lancer la base de données avec la commande
    - sudo docker compose up -d
    - sudo docker compose down -> pour fermer les containers
- Rentre l'adresse ip avec le port exposer pour tester BD
    - ex. http://10.10.0.0:8080
- Fonctionnment principale
  + Lancer le cluster
    - kubectl apply -f mistify-manifests/mistify-frontend/
    - kubectl apply -f mistify-manifests/mistify-backend/
  + Arrête le cluster
    - kubectl delete -f mistify-manifests/mistify-frontend/
    - kubectl delete -f mistify-manifests/mistify-backend/
