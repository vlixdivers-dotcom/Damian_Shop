Header : 
Logo 
Menu avec les différentes catégories 

Page principale : 
Slider avec différents liens "sélection du jour " 
Des previews des articles par catégorie 

Page produit : 
Photo 
Nom 
Descriptions 
Note 
Avis 

Page panier : 
Liste des articles avec quantité et prix total 
Enregistrer sur le local storage 

Page de paiement : 
Splice 

Page admin : 
Liste des stocks et produits 
CRUD produit 

Bdd : 
Postgres 


Dev: 
Serveur Marcel 
Docker compose  php, nginx, postgres 

Prod : 
À voir avec Aymeric 

Versioning : 
Git 

À prévoir : 
Identification (email, password, verif email), 
Fixtures,
Test unitaire, 
Stockage interne des photos 

--- 

Catégorie : 
Id,
Nom (slug)

Entité : 
id,
Nom (slug)
Description
Prix 
Photo
FK_categorie id 

Route : 

User : 
Homepage - /
Display - /display/{category_id}
Product detail - /product/{product_id}
Login - /login 
Sign up - /sign-up

Member : 
Profil - user/{usr_id}
panier - /cart

Admin : 

---
Conception:
Maquette fonctionnelle figma 
Définition structure bdd 
Installation environnement technique 

Prototype: 
Création des entités 
Fixtures 
Création des routes
Achat fictif