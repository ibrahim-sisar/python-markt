# Super Market Invoice Management System

This project is a Python-based graphical user interface (GUI) application built using the `Tkinter` library, and it is designed to manage product inventories, customer invoices, and barcode scanning for a supermarket. The system allows users to:

- Add and manage products.
- Scan barcodes to retrieve product information.
- Generate and save customer invoices.
- Calculate and display the total amount of the invoice.
- Search, edit, and delete customer invoices.

## Features

- **Product Management**: 
  - Add products by scanning barcodes or manually entering product details (name, price).
  - Store product data in an Excel file (`excel/ib.xlsx`).
  
- **Barcode Scanning**:
  - Use a webcam to scan product barcodes with real-time feedback.
  - Automatically retrieve product information (name, price) based on the barcode scanned.

- **Invoice Generation**:
  - Generate invoices with customer details (name, address, phone number).
  - Automatically calculate the total amount based on selected products.
  - Save invoices to an Excel file (`customers.xlsx`).

- **Invoice Management**:
  - Search for customer invoices by name.
  - Edit and delete customer invoices.

- **GUI Interface**:
  - Simple and user-friendly interface built using Tkinter.
  - Includes buttons to perform operations like saving, clearing, calculating totals, and deleting invoices.

## Installation

To run this project, you will need to install the following dependencies:

1. **Python 3.x** (Ensure Python is installed on your system)
2. Install the required Python libraries:
    ```bash
    pip install opencv-python pyzbar Pillow openpyxl pyttsx3
    ```

## Usage

### Run the Application

1. Download or clone the repository to your local machine.
2. Open a terminal or command prompt in the project directory.
3. Run the application using the following command:
    ```bash
    python m.py
    ```

### Barcode Scanning

- Click the "مسح الباركود" button to activate the barcode scanning feature.
- Point your camera at the barcode of a product, and the system will automatically fill in the product name and price.

### Managing Products

- Use the "حفظ المنتج" button to add a new product by entering its barcode, name, and price.
- Use the "إضافة للجدول" button to add the product to the invoice table.

### Managing Invoices

- Use the "حفظ الفاتورة" button to save an invoice once products have been added.
- Use the "حساب الإجمالي" button to calculate the total price of the invoice.
- Use the "مسح الحقول" button to clear the form fields and the invoice table.
- Use the "حذف الفاتورة" button to delete an existing invoice.

## Files and Directories

- **main.py**: The main application file that runs the system.
- **customers.xlsx**: Excel file that stores customer information and invoices.
- **excel/ib.xlsx**: Excel file that stores product information (barcode, name, price).
- **img/ico/market.ico**: Application icon.
- **img/png/logo4.png**: Application logo.

## License

This project is open-source and available under the [MIT License](LICENSE).

## Acknowledgements

- The project uses `opencv-python` for webcam functionality and `pyzbar` for barcode scanning.
- The project uses `openpyxl` for handling Excel files and `tkinter` for the GUI.
- Special thanks to the contributors of these libraries for making this project possible.

