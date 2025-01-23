# Cookie-Land
Repo to map building Cookie Land Bakery business

## This is how I plan to Make Cookie Profits

In this repo I lay out my plans to sell many cookies.
To flood the market with remarkable cookie flavors. To build my cookie Empire. Follow my rise to cookie stardom.

# My Customer Relationship

## Flow Chart to Explain Purchase from Cookie Land

```mermaid
erDiagram

Customer ||--|| Payment : transaction
Payment ||--o{ Product : select
Payment }|--|| Profit : BusinessGrowth
Product }|--|| Retail : CookieLand
Retail ||--|| Profit : CheapProduct
CUSTOMER {
        string customerID PK
        string name
        string email
    }
    
PAYMENT {
        string customerID PK
        string name
        string paymenttype
    }
    PRODUCT {
        string customerID PK
        string flavor
        string quantity
}

```
thus it begins