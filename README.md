
# Cinema Paradiso

## Overview

Cinema Paradiso is a project designed to manage and simulate the pricing and ordering process of cinema tickets. The system includes functionalities such as calculating ticket prices based on various criteria, managing orders, and generating receipts.

## Setup Instructions

### Prerequisites

- PHP (version 7.4 or higher recommended)
- A web server (such as Apache or Nginx)
- Composer (for managing PHP dependencies)

### Steps

1. **Clone the Repository**

   ```bash
   git clone https://github.com/yourusername/cinema-paradiso.git
   cd cinema-paradiso
   ```

2. **Install Dependencies**

   If you have any dependencies managed by Composer, install them:

   ```bash
   composer install
   ```

3. **Configure the Project**

   - Update any necessary configuration settings in the project files. This might include database configurations, API keys, etc.

4. **Run the Project**

   - Place the project files in your web server's root directory.
   - Access the project through your web browser (e.g., `http://localhost/cinema-paradiso/start.php`).

## Project Structure and Description

### Files

1. **start.php**
   
   The main entry point of the project. Initializes the system and sets up the necessary components to simulate the cinema ticket ordering process.

2. **CinemaPriceEngine.php**

   Handles the logic for calculating cinema ticket prices. It includes various pricing rules and criteria to determine the final ticket price.

3. **OrderCollection.php**

   Manages a collection of `Order` objects. Provides functionalities to add, retrieve, and manage multiple orders.

4. **Order.php**

   Defines the `Order` class. This class includes properties and methods related to a cinema ticket order, such as ticket details and customer information.

5. **ReceiptGenerator.php**

   Handles the generation of receipts for the orders. It takes order details and formats them into a receipt that can be printed or displayed.

6. **PriceCalculator.php**

   A utility class used by the `CinemaPriceEngine` to perform various price calculations. It might include methods for applying discounts, calculating taxes, and more.

## Project Flow

1. **Initialization:**
   - `start.php` initializes the project and sets up the necessary components.

2. **Order Management:**
   - Orders are managed through `Order.php` and `OrderCollection.php`.

3. **Price Calculation:**
   - The price of cinema tickets is calculated using `CinemaPriceEngine.php` and `PriceCalculator.php`.

4. **Receipt Generation:**
   - Receipts are generated and formatted using `ReceiptGenerator.php`.
