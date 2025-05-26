```mermaid
---
title: Nike Shoe Store
---
erDiagram


  PRODUCT }o--||INVENTORY : in
  PRODUCT {
    string product_name
    int quantity
    float pricePerUnit
  }
  CUSTOMER ||..|{ SALE : makes_a_purchase
  CUSTOMER {
    string firstName
    string lastName
    int age
  }
  SALE ||--|| CUSTOMER : made_by
  SALE {
    int numOfProducts
    float priceOfSale
  }
  INVENTORY ||..|{ SALE : exchanges_product_for
  INVENTORY {
    int numOfDistinctProducts
    
  }
```
