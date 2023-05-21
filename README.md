# Books QR Code Generator and Database Insertion

This is a Python script that generates QR codes for book details and inserts the information into a MySQL database. Each record represents a book and includes various attributes such as the owner, purchase date, book name, author, publisher, book code, and date finished.

## Prerequisites

Before running the script, make sure you have the following installed:

- Python 3.x
- MySQL connector for Python (`mysql-connector-python`)

You can install the MySQL connector by running the following command:

```
pip install mysql-connector-python
```

## Usage

1. Clone the repository or download the script directly.
2. Set up a MySQL database with the appropriate table structure. The table structure should match the `DETAILS` table used in the script. Make sure to update the database connection details (host, user, password, database) in the script to match your MySQL configuration.
3. Run the script using the following command:

```
python script.py
```

4. When prompted, enter the number of records you want to insert.
5. For each record, enter the required book details as requested.
6. The script will insert the record into the database and generate a QR code image file named after the book name and author.
7. The generated QR code image files will be saved in the same directory as the script.

## Example

Here's an example interaction with the script:

```
No of Records to be Inserted : 1
Owner : John
Date Purchased : 2023-05-20
Book Name  : Introduction to Python
Author : Jane Doe
Publisher : ABC Publications
Book Code : 12345
Date Finished : 2023-05-21
Introduction to Python Jane Doe.jpeg
```

In this example, a single record is inserted into the database with the provided book details. The corresponding QR code is generated and saved as "Introduction to Python Jane Doe.jpeg" in the same directory.

Note: Make sure to customize the script according to your specific requirements, such as table name, field names, and database configuration.
