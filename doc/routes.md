##Routes

User :

- Homepage - /
-Display - /display/{category_id}?type=[all,cdb,cbc]
-Product detail - /product/{product_id}
-Login - /login 
-Sign up - /sign-up

Member : 

-Profil - user/{usr_id}
-panier - /cart


Admin : 

- Dashboard - /dashboard
- Dashboard Display - /dashboard/display?category=[all,fleurs,resine,edibles]+type=[all,cdb,cbc]
- Edit Product - /product/edit/{product_id}
- *Delete Product - /product/delete/{product_id}* 
- *Add product - /product/add/{json-product-infos}*
