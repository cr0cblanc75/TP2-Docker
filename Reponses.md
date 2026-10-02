## Question 2-1
"testcontainers" créer un container de test pour effectuer des tests de code dedans. 

## Question 2-2
On ajoute jamais de données sensibles sur gitHub, simplement car le `repo` pourrait être en public, et donc être visible par tout le monde. Pour des raisons assez évidentes de sécurité, on ne partage pas de mot de passe ni d'identifiant. On va donc utiliser le conteneur workflows sécurisé de github.

## Question 2-3
On doit utiliser `needs: test-backend ` pour faire l'image Docker, car on veut être sûr que le test qu'on fait sur le backend soit bon et validé, avant de créer des images et de les publier.