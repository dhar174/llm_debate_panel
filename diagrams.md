


```mermaid
erDiagram
    CUSTOMERS {
        int id
        string name
        string age_band
        string region
    }
    ORDERS {
        int id
        int customer_id
        int product_id
        int quantity
    }
    PRODUCTS {
        int id
        string category
        number price
    }

    CUSTOMERS ||--o{ ORDERS     : places
    ORDERS     }o--|| PRODUCTS   : contains
 
```
