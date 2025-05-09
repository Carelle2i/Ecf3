Documentation pour la Construction et le Démarrage de l'Application avec Docker et Docker Compose


Après avoir mis en place les dockerfile et docker-compose, j'ai lancé la commande : docker-compose up --build pour construire les images Docker et démarer tout les services.

Une fois l'application démarer, j'ai pu accéder à l'interface utilisateur (UI) React dans mon navigateur à l'adresse suivante http://localhost:3000
et ensuite tester le bon fonctionnement de l'application et que les différents appels se font bien comme il le faut.

Je peux aussi acceder à l'interface utilisateur et utiliser la barre de recherche pour saisir un terme.

L'UI va envoyer une requête à l'API du microservice de recherche pour récupérer des suggestions basées sur la saisie de l'utilisateur.

Pour vérifier la communication, je vais consulter les logs,par exemple j'utilise cette commande : docker logs common-data-service-container pour vérifier si le microservice de recherche se connecte bien à la bdd.
