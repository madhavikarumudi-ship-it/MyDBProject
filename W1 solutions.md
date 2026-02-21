***Here is Question (W1-P1.1)***
**Given: Requirements for an e-commerce system: customers browse products, place orders with multiple items, pay, and receive shipment updates. Task: Identify entities/relationships, specify cardinalities, and list 10 integrity rules (e.g., “an order must have ≥1 item”, “product stock cannot be negative”).**

**1. Entities** 
- Customer (CustomerID, Name, Email, Phone, Address)
- Product (ProductID, ProductName, Description, Price, StockQuantity)
- Order (OrderID, Date, OrderStatus, TotalAmount)
- OrderItem (OrderID, ProductID, Quantity, ItemPrice)
- Payment (PaymentID, OrderID, PaymentDate, Amount, PaymentMethod, PaymentStatus)
- Shipment (ShipmentID, OrderID, ShipmentDate, TrackingNumber, DeliveryStatus)
  
**2. Relationships & Cardinalities**
  - Customer – Order (1:M)
  - Order – OrderItem (1:M)
  - Product – OrderItem (1:M)
  - Order – Payment (1:1)
  - Order – Shipment (1:M) or (1:1)
    
  **3. Integrity Rules (10 Constraints)**
    
