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

    class User : Entity{
        + email
        + password #
        + username
        + FK-user_contact_information_id (delivery)       
        + FK-user_contact_information_id (facturation) 
        + FK-user_bank_information_id 
        + creation_date
    }

    class UserCoordinates{
        + id
        + adress
        + postal_code
        + town
        + country
        + first_name
        + last_name
        + phone_number
        + creation_date
    }

    class  UserBankInformation{
        + id 
        + card_number #
        + cvs #
        + first_name
        + last_name
        + creation_date
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