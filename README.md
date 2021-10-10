##Objectifs :
● Créer et manipuler un composant
● Appliquer le databinding (event-binding, property-binding, two-way databinding)
● Définir un modèle de données
● Manipuler les directives NgFor

##Etude de cas:
Nous souhaiterions créer une application E-Commerce en utilisant le framework Angular côté frontEnd. Sachant que la partie opérationnelle (la couche métier) est déjà développée et elle est exposée sous forme des services web côté backend.
Créer une SPA (Single Page Application) permettant à l’utilisateur de:
a. parcourir une liste de produits
b. commander un produit,
c. liker un produit,
d. de chercher un produit par prix.
Travail à faire :
1. Créer un projet Angular

2. Créez un composant appelé ProductsComponent.

3. Créez un modèle de données appelé « Product » à définir sous un répertoire model comme suit : export class 

Product{ id:string; title:string;price:number; quantity:number ; like:number; }
}

4. Afficher la liste des produits définis dans la propriété productList du composant créé: listProdcut=[ {id: 1, title: "T-shirt 1", price: 18, quantity: 0, like: 0}, {id: 2, title: "T-shirt 2", price: 21, quantity: 10, like: 0}, {id: 3, title: "T-shirt 3", price: 16, quantity: 8, like: 0}, ]

5. Ajouter deux boutons « Buy » et « like » devant chaque Produit.

6. Le bouton « Buy » est inactif si la quantité du produit est égale à 0 .

7. Le clique sur le bouton « Buy » permet de décrémenter la quantité du produit sélectionné.

8. Le clique sur le bouton like permet d’incrémenter le nombre de like du produit sélectionné.

9. Ajouter un input de type « number » qui permet à l’utilisateur de chercher les produits dont le prix est inférieur au prix taper dans le champ.