# **Practical Assignment 01**

**_Purpose_**: Practice with writing select queries.

### Basic requirements:

Write complex select with joining 5 tables,
using where clause. 
Be able to explain your solution using the correct terminology.
5 points


### Additional points:

Source code published in GitLab +0.5
Union or union all +0.5
CTE + 1

### Helper

`script.sql` file can help you with syntax. This is simplified example of your assignment.
_You **can not** use the same tables structure in your assignment._

ERD:
```mermaid
erDiagram
    CLIENTS {
        int ClientID PK
        varchar ClientName
        varchar Email
        varchar Phone
    }
    
    PRODUCTS {
        int ProductID PK
        varchar ProductName
        decimal Price
    }
    
    ORDERS {
        int OrderID PK
        int ClientID FK
        int ProductID FK
        date OrderDate
        int Quantity
    }
    
    CLIENTS ||--o{ ORDERS : places
    PRODUCTS ||--o{ ORDERS : includes
```
