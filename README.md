# Cookie-Land
Repo to map building Cookie Land Bakery business

## This is how I plan to Make Cookie Profits

In this repo I lay out my plans to sell many cookies.
To flood the market with remarkable cookie flavors. To build my cookie Empire. Follow my rise to cookie stardom.

# My Customer Relationship

## Flow Chart to Explain Purchase from Cookie Land

```mermaid


erDiagram
    CUSTOMER ||--|| PAYMENT_TYPE : "Debit/Credit Card"
    PAYMENT_TYPE ||--o{ COOKIE_CHOICE : "customer selection"
    COOKIE_CHOICE }|--|| COOKIE_PRODUCTION : "Ingredient/Material"
    COOKIE_PRODUCTION }|--|{ COOKIE_CHOICE : "customer selection"
    RETAIL_STORE }|--|| PROFIT : "Preferred pricing Options"
    PROFIT ||--o{ BAKERS_OTHER_STAFF_UTILITIES : "BusinessOverhead"
    BAKERS_OTHER_STAFF_UTILITIES ||--|{ COOKIE_PRODUCTION : "Develop New Flavors"
    CUSTOMER {
        string customerid PK
        string name
        string email
        string address
        string cardinfo 

    }
    
    "PAYMENT_TYPE" {
        string customerID PK
        string cardNumber
        }
    
    COOKIE_CHOICE {
        string customerID PK
        string flavor
        string quantity
    }
    
    note {
        
    }
    
   
       
    end
