

'''mermaiderDiagram
  PRODUCT }o--||INVENTORY : in
  PRODUCT {
    string product_name
    int quantity
    float pricePerUnit
  }
  CUSTOMER ||..|{ SALE : makes a purchase
  CUSTOMER {
    string firstName
    string lastName
    int age
  }
  SALE ||--|| CUSTOMER : made by
  SALE {
    int numOfProducts
    float priceOfSale
  }
  INVENTORY ||..|{ SALE : exchanges product for
  INVENTORY {
    int numOfDistinctProducts
    
  }
