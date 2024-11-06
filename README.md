# cpl

dbms connection code 

# pip install mysql-connector-python
import mysql.connector

# Connect to the database
connection = mysql.connector.connect(
    host="localhost",       # Replace with your MySQL server, usually 'localhost'
    user="your_username",   # Replace with your MySQL username
    password="your_password",  # Replace with your MySQL password
    database="your_database"   # Replace with your database name
)

# Check if the connection is successful
if connection.is_connected():
    print("Connected to the database!")

# Close the connection
connection.close()
