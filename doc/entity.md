## Entitées sauvegardé en BDD (postgres)

    class Category{
        + id
        + nom 
    }

    class Type{
        + id
        + nom 
    } 


    class Entity{ 
        + id,
        + Nom (slug)
        + creation_date 
    }

    class Product : Entity{
        + Description
        + Prix 
        + Photo
        + FK-categorie_id 
        + FK-type_id 
    }

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

    class User : Entity{
        + email
        + password #
        + username
        + FK-user_contact_information_id (delivery)       
        + FK-user_contact_information_id (facturation) 
        + FK-user_bank_information_id 
        + creation_date
    }

    class UserContact_information{
        + id
        + adress
        + postal_code
        + town
        + country
        + first_name
        + last_name
        + phone_number
        + creation_date
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

    class UserOrder{
        + FK-user_id
        + FK-order_id
        + FK-delivery_information_id
    }

    class Order{
        + id
        + FK-product_id []
        + creation_date
        + FK-order_status_id
    }

    class Order_Status{
        + id
        + name
    }

    class DeliveryInformation{
        + id
        + FK-user_contact_information_id (client)
        + FK-user_contact_information_id (postman)
        + FK-DeliveryStatus_id
    }

    class DeliveryStatus{
        + id
        + name
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


