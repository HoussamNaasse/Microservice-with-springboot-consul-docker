Tutoriel sur l'utilisation de Microservices avec Consul et Docker
Ce tutoriel vous guidera à travers la mise en place d'une architecture de microservices en utilisant Consul pour la découverte de services et Docker pour le déploiement. Les quatre principaux services inclus sont :

Service Client

Agit comme un point d'entrée pour les demandes des utilisateurs.
Interagit avec d'autres services pour répondre aux requêtes.
Service Voiture

Gère les informations relatives aux voitures, telles que la création, la modification et la suppression des données des véhicules.
Service de Découverte (Discovery)

Utilise Consul comme serveur de découverte pour permettre aux services de trouver et de se connecter de manière dynamique.
Service Passerelle (Gateway)

Agit comme une passerelle pour rediriger les requêtes des utilisateurs vers les services appropriés.
Comment Utiliser ce Tutoriel
Prérequis
Docker installé sur votre machine.
Compréhension de base des microservices et de Consul.
Simulation
Consultez la simulation du tutoriel ici.

Étapes du Tutoriel
Clonez ce dépôt Git sur votre machine locale.
Accédez à chaque service individuellement pour comprendre son rôle et son fonctionnement.
Suivez les instructions de déploiement pour exécuter l'ensemble des services sur Docker.
Instructions de Déploiement
Accédez au répertoire racine du projet.
Exécutez docker-compose up pour démarrer l'ensemble des services.
Consultez les logs pour vous assurer que tous les services se sont correctement démarrés.
Endpoints API
Dashboard Consul : http://localhost:8500/ui/dc1/services
PhpMyAdmin : http://localhost:8081/ (root:root)
Service Client
Récupérer tous les clients : GET http://localhost:8888/SERVICE-CLIENT/clients
Ajouter un nouveau client : POST http://localhost:8888/SERVICE-CLIENT/clients
Mettre à jour un client existant : PUT http://localhost:8888/SERVICE-CLIENT/clients/{id}
Supprimer un client : DELETE http://localhost:8888/SERVICE-CLIENT/clients/{id}
Service Voiture
Récupérer toutes les voitures : GET http://localhost:8888/SERVICE-VOITURE-V0/voitures
Ajouter une nouvelle voiture : POST http://localhost:8888/SERVICE-VOITURE-V0/voitures
Mettre à jour une voiture existante : PUT http://localhost:8888/SERVICE-VOITURE-V0/voitures/{id}
Supprimer une voiture : DELETE http://localhost:8888/SERVICE-VOITURE-V0/voitures/{id}




https://github.com/HoussamNaasse/Microservice-with-springboot-consul-docker/assets/118965865/c43abce7-801e-4022-bf4a-b83cc21c3ada




