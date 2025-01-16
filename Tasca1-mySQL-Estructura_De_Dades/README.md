For each exercise in this task ("tasca"), it was required to deliver two things: 
1. Relational model with the database design. If you wish, you can use draw.io, dbdiagram.io, Mysql Workbench or any other tool that allows you to draw the structure and export it in png or jpg format (to upload it to the repository). We especially recommend genmymodel.com.
2. Script .sql of the database creation and data insertion. 

# Exercise Guidelines

- ## Exercise 1 - Optical

    An optical shop, called “Cul d’Ampolla”, wants to computerize the management of customers and glasses sales.
    
    First of all, the optical wants to know who is the supplier of each of the glasses. Specifically, you want to know from each supplier:
    - The name
    - The address (street, number, floor, door, city, postal code and country)
    - Phone
    - Fax
    - NIF.
    
    The optical purchasing policy is based on the fact that the glasses of a brand will be bought from a single supplier (thus you can get better prices), but you can buy glasses of several brands from a supplier. From the glasses you want to know:
    - The brand.
    - The graduation of each of the glasses.
    - The type of mount (floating, pasta or metal).
    - The color of the mount.
    - The color of each glass.
    - The price.
    
    From the customers/to be stored:
    - The name.
    - The postal address.
    - The phone.
    - The email.
    - The date of registration.
    - When a new customer arrives, store the customer who has recommended the establishment (as long as someone has recommended it).
    - Our system must indicate who has been the employee who has sold each glasses.
    
- ## Exercise 2 - Pizzeria

    They have hired you to design a website that allows you to place food orders at home online.
    
    Keep in mind the following indications to model what the project database would be like:
    - For each client we store a unique identifier:
        - Name.
        - Last name.
        - Address.
        - Postal code.
        - Locality.
        - Province.
        - Phone number.
        - Locality and province data will be stored in separate tables. We know that a locality belongs to a single province, and that a province can have many localities. For each location we store a unique identifier and a name. For each province we store a unique identifier and a name.
    
    - A person can place many orders, but a single order can only be made by a single person. From each order a unique identifier is stored:
        - Date/Time.
        - If the order is for home delivery or to pick up in store.
        - The number of products selected for each type.
        - The total price.
    
    An order may consist of one or more products.
    
    - The products can be pizzas, burgers and drinks. A unique identifier is stored for each product:
        - Name.
        - Description.
        - Image.
        - Price.
    
    In the case of pizzas there are several categories that can be renamed throughout the year. A pizza can only be in one category, but a category can have many pizzas.
    
    - A unique identifier and a name are stored in each category. An order is managed by a single store and a store can handle many orders. From each store a unique identifier is stored:
        - Address.
        - Postal code.
        - Locality.
        - Province.
    
    - In a store many employees can work and an employee can only work in a store. For each employee, a unique identifier is stored:
        - Name.
        - Last name.
        - NIF.
        - Phone.
        - If you work as a cook or delivery company, it is important to store who is the delivery company who delivers the order and the date/time of the delivery.
