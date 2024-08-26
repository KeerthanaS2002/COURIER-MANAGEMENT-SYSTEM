Courier Management System:

This Courier Management System is a Python-based application that allows users to manage courier services through a graphical user interface (GUI) built with Tkinter.
The system connects to a MySQL database to store and retrieve information about customers and their couriers.

Key Features:

1.User Registration and Login:
   - Users can register with their first name, last name, registration number,phone number and a password.
   - The system ensures that all fields are filled and that the passwords match before allowing registration.
   - Registered users can log in using their registration number and password.

2.Courier Management:
   - After logging in, users can add new couriers by providing the receiver's name,address and phone number.
   - The system automatically assigns a unique ID to each courier and sets its status to "In Transit."

3.Courier Tracking:
   - Users can track the status of their couriers by entering the courier ID.
   - The system retrieves and displays the courier's current status,as well as information about the sender and receiver.

4. Status Updates:
   - Users can update the status of a courier by entering the courier ID and the new status (e.g:"Delivered").

5. Database Management:
   - The application connects to a MySQL database, creating necessary tables for customers and couriers if they don't already exist.
   - The `customers` table stores user information, including a unique registration number and encrypted passwords.
   - The `couriers` table stores information about each courier,including the sender's ID (linked to the customer),receiver details and the current status of the courier.

Setup Instructions:

1.Install Required Libraries:
   * Make sure to install the necessary Python libraries:
     pip install mysql-connector-python pillow
2.Database Configuration:
   * The system is set up to connect to a local MySQL database. Update the `setup_database` function with your MySQL credentials if needed.

3.Running the Application:
   * Run the script, and the application will start with the login page.
   * You can then register as a new user, log in, and begin managing couriers.

This system is ideal for small businesses or personal use, where tracking and managing deliveries are essential.
The user-friendly interface ensures that all operations can be performed easily, making it a practical solution for courier management needs.
