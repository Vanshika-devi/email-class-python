# email-class-python
Email System Simulator
A lightweight Python application that simulates a basic email exchange system. This project demonstrates core Object-Oriented Programming (OOP) concepts, including class interaction, encapsulation, and list management.

## Features
User Management: Create multiple users with unique names.

Email Creation: Automatically generates timestamps and tracks "Read/Unread" status.

Inbox Functionality: Users can receive, list, read, and delete emails.

Inter-User Communication: Seamlessly send messages from one User object to another.

## Class Structure
The system is built on three primary classes:

Email: Stores metadata (sender, receiver, subject, body, timestamp) and manages the display format of individual messages.

Inbox: Acts as a container for Email objects, providing methods to organize and manipulate the collection of messages.

User: The high-level interface that allows a person to send emails and access their personal inbox.

## Getting Started
### Prerequisites
Python 3.x installed on your machine.

### Running the Simulation
Copy the code into a file named email_system.py.

Open your terminal or command prompt.

Run the script using:

Bash
python email_system.py
## Example Usage
The main() function provides a built-in demonstration of the system:

Python
# Create users
tory = User('Tory')
ramy = User('Ramy')

# Send emails
tory.send_email(ramy, 'Hello', 'Hi Ramy, just saying hello!')

# Check and read emails
ramy.check_inbox()
ramy.read_email(1)

# Manage messages
ramy.delete_email(1)
## Future Improvements
Add a Drafts folder for unsent emails.

Implement a Search feature to find emails by subject or sender.

Add a Command Line Interface (CLI) to allow real-time user input instead of hardcoded simulation.
