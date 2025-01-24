# Cookie-Land
Repo to map building Cookie Land Bakery business

## This is how I plan to Make Cookie Profits

In this repo I lay out my plans to sell many cookies.
To flood the market with remarkable cookie flavors. To build my cookie Empire. Follow my rise to cookie stardom.

# My Customer Relationship

## Flow Chart to Explain Purchase from Cookie Land

```mermaid
erDiagram
    CUSTOMER ||--|| "PAYMENT TYPE" : "Debit/Credit Card"
    "PAYMENT TYPE" ||--o{ COOKIES : "select"
    COOKIES }|--|| RETAIL : "Ingredient/Material"
    RETAIL }|--|| PROFIT : "Preferred pricing"
    PROFIT ||--|| "BAKERS & OTHER STAFF" : "BusinessOverhead"
    PROFIT ||--o{ COOKIES : "Develop New Flavors"
    CUSTOMER {
        string customerid PK
        customerid name
        customerid email
    }
    
    "PAYMENT TYPE" {
        string customerID PK
        string name
        string cardNumber
        string paymentType
    }
    
    COOKIES {
        string customerID PK
        string flavor
        string quantity
    }
    
    ENTITY {
        string name
    }
    
    note right of ENTITY
        note content
    end
