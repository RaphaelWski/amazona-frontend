# Amazona: frontend

## Getting started

Cloner le projet puis executer les commandes suivantes

### `npm install`

### `npm start`

Ouvrez votre navigateur à l'adresse suivante [http://localhost:3000](http://localhost:3000)

> Note: démarrer au préalable le serveur web (projet backend)

## Informations

Présentation du contenu :

### User
La base de données contient 3 utilisateurs dont un Administrateur (Oda)

```json
[{
  "_id": {
    "$oid": "5ed7c4a8d098762144f699cd"
  },
  "isAdmin": true,
  "name": "Oda",
  "email": "oda@gmail.com",
  "password": "password",
  "__v": 0
},{
  "_id": {
    "$oid": "5ed7f1bef1e6482b58df3487"
  },
  "isAdmin": false,
  "name": "Luffy",
  "email": "Monkey.D.Luffy@gmail.com",
  "password": "password",
  "__v": 0
},{
  "_id": {
    "$oid": "5ed94a417dd85001f445abeb"
  },
  "isAdmin": false,
  "name": "Zoro",
  "email": "RoronoaZoro@gmail.com",
  "password": "password",
  "__v": 0
}]
```

### Products

```json
[{
  "_id": {
    "$oid": "5ed955697dd85001f445abed"
  },
  "price": 10,
  "countInStock": 10,
  "name": "Cotton Fit Shirt",
  "image": "/images/d3.jpg",
  "brand": "Hast",
  "category": {
    "$oid": "5ed8ed7d0cfa384bb8f0cd02"
  },
  "description": "This is a Cotton Fit Shirt",
  "__v": 0
},{
  "_id": {
    "$oid": "5ed9557c7dd85001f445abee"
  },
  "price": 10,
  "countInStock": 10,
  "name": "Classic shirt",
  "image": "/images/d2.jpg",
  "brand": "Boss",
  "category": {
    "$oid": "5ed8ed7d0cfa384bb8f0cd02"
  },
  "description": "This is a Classic shirt",
  "__v": 0
},{
  "_id": {
    "$oid": "5eda00759d732749a025244f"
  },
  "price": 100,
  "countInStock": 10,
  "name": "Slim Shirt",
  "image": "/images/d1.jpg",
  "brand": "Lacoste",
  "category": {
    "$oid": "5ed8ed7d0cfa384bb8f0cd02"
  },
  "description": "This is a Slim Shirt",
  "__v": 0
},{
  "_id": {
    "$oid": "5eda69345018d306c8ed2187"
  },
  "image": "/images/h1.jpg",
  "price": 100,
  "countInStock": 10,
  "name": "Luffy's Hat",
  "brand": "GrandLine",
  "category": {
    "$oid": "5ed92cc30cfa384bb8f0cd04"
  },
  "description": "This is One piece Luffy's Hat",
  "__v": 0
},{
  "_id": {
    "$oid": "5eda69a05018d306c8ed2188"
  },
  "image": "/images/h2.jpg",
  "price": 10,
  "countInStock": 2,
  "name": "Zoro's Hat",
  "brand": "RedLinde",
  "category": {
    "$oid": "5ed92cc30cfa384bb8f0cd04"
  },
  "description": "This is Zoro's Hat",
  "__v": 0
},{
  "_id": {
    "$oid": "5eda6a575018d306c8ed2189"
  },
  "image": "/images/p1.jpg",
  "price": 100,
  "countInStock": 4,
  "name": "Cotton Pants",
  "brand": "Lacoste",
  "category": {
    "$oid": "5ed92cba0cfa384bb8f0cd03"
  },
  "description": "This is a Cotton Pants",
  "__v": 0
},{
  "_id": {
    "$oid": "5eda6a865018d306c8ed218a"
  },
  "image": "/images/p2.jpg",
  "price": 49,
  "countInStock": 12,
  "name": "Slim Pants",
  "brand": "Boss",
  "category": {
    "$oid": "5ed92cba0cfa384bb8f0cd03"
  },
  "description": "This is a Slim Pants",
  "__v": 0
}]
```

### Categories

```json
[{
  "_id": {
    "$oid": "5ed8ed7d0cfa384bb8f0cd02"
  },
  "name": "Shirts",
  "__v": 0
},{
  "_id": {
    "$oid": "5ed92cba0cfa384bb8f0cd03"
  },
  "name": "Pants",
  "__v": 0
},{
  "_id": {
    "$oid": "5ed92cc30cfa384bb8f0cd04"
  },
  "name": "Hats",
  "__v": 0
}]
```

Vous pouvez utiliser le compte suivant pour la sandbox Paypal
```
  email: sb-qvpkt2185464@personal.example.com
  password: Sc=c5C3%
```

### Fonctionnalités

Voici un récapitulatif des fonctionnalités demandés :

- Articles :white_check_mark:
- Catégories :white_check_mark:
- Panier :white_check_mark:
- Achat fictif :white_check_mark:
- Utilisation d'une API externe : 
  - Paypal :white_check_mark:
- Front Office :
  - Recherche :white_check_mark:
- Back Office :
  - CRUD simples pour les Articles / Catégories :white_check_mark:
  - Total chiffre d'affaire par jour :x:
  - Top Articles et top Catégories :x:
- API Back
  - Endpoint de récupération en JSON des top Articles et top Catégories :x: