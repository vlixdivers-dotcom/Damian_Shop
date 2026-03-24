## Entitées sauvegardé en BDD (postgres)


    class Category{
        + id
        + name 
    }

    class Type{
        + id
        + name 
    } 

    class Effect{
        + id 
        + name
    }


    class Entity{ 
        + id
        + name
        + creation_date 
    }

    class Product : Entity{
        + description
        + price
        + image_url
        + FK-category_id 
        + FK-type_id 
    }

<<<<<<< HEAD:doc/classDiagram.md
    class ProductEffect{
        + id
        + product_id
        + effect_id
    }

    class Review{
        + id
        + fk-user_id
        + fk-product_id
        + notation
    }
=======
class Notation{
+id
+ note 
}

class Review {
+ id 
+ author_id 
+ header 
+ body 
+ creationDate 
}

class ProductReview{
+ id 
+ product_id
+ review_id 
}

class ProductNotation{
id
product_id
notation_id
}
>>>>>>> 726cbd7e0d92ecdfb61904d6e5f8c3b76df1eba3:doc/entity.md

    class User : Entity{
        + email
        + first_name
        + last_name
        + phone_number
        + password #
        + username
        + creation_date
    }

    class UserDeliveryAdress{
        + id 
        + adress
        + postal_code
        + town
        + country
        + details
        + FK-user_id
    }

    class UserBillingAdress{
        + id
        + adress
        + postal_code
        + town
        + country
        + details
        + FK-user_id
    }

    class  UserBankInformation{
        + id 
        + card_number #
        + cvs #
        + first_name
        + last_name
        + creation_date
        + FK-user_id
    }

    

    class Order{
        + id
        + creation_date
    }

    class ProductOrder{
        + id
        + FK-order_id
        + FK-product_id  
    }

    class UserOrder{
        + FK-user_id
        + FK-order_id
        + FK-delivery_information_id
    }

    class OrderStatus{
        + id
        + name
        + FK-order_id
    }


    class  EmailSent{
        + id 
        + subject
        + body
        + sender_email
        + receiver_email
        + creation_date
    }

    class Log{
        + id
        + subject
        + body
        + FK-log_type_id
    }

    class LogType{
        + id
        + name
        + code
    }


