# Comment faire fonctionner l'application:

pour lancer l'application, il y a deux manières:


## Premiere manière:

La premiere maniere est de récupérer l'image depuis dockerHub grace à la commande:

docker push gillesdegue/flaskapp:tagname

puis lancer le container avec la commande 

docker run --name flaskapp -p 5000:5000 flaskapp

puis se rendre sur l'adresse localhost:5000 pour visualiser le resultat


## deuxième manière:

éffectuer un pull depuis github grace a la commande:

git clone git@github.com:gillesdegue/flaskApp.git

une fois dans le répertoire du projet cree l'image en effectuant la commande :

docker build -t flaskapp .

puis lancer le container avec la commande:

docker run --name flaskapp -p 5000:5000 flaskapp

puis se rendre sur l'adresse localhost:5000 pour visualiser le resultat
