# Cinema Ticket Booking System

- [Description](#description)
- [Database Schema](#database-schema)
- [Code Overview](#code-overview)
- [How to Use](#how-to-use)
  - [Pre-requisites](#pre-requisites)
  - [Steps](#steps)
- [Contributing](#contributing)
- [License](#license)

## Description

This project is a cinema ticket booking system developed using C# and various technologies like Entity Framework Core, WPF, and SQL Server. It enables users to view available cinemas, movie screenings, and purchase tickets for specific movie showings at different cinema locations.

## Database Schema

The database consists of four main tables:

- **Cinemas:** Stores information about cinema locations.
- **Movies:** Contains details about different movies including title, runtime, release date, and poster path.
- **Screenings:** Holds data about movie screenings at specific cinemas with their timings.
- **Tickets:** Stores information about purchased tickets including the screening ID and purchase time.

The SQL Server database schema enforces relationships between these tables to maintain data integrity and ensure accurate information storage.

## Code Overview

The project is divided into three main sections:

1. **Database Population Tool (`PopulateDatabase`):** A C# program that reads CSV files containing movie and cinema information and populates the SQL database tables accordingly.
2. **Entity Framework Core Classes (`Assignment3`):** Contains classes representing database entities like Cinemas, Movies, Screenings, and Tickets. These classes are utilized by the WPF application to interact with the SQL database.
3. **WPF Application (`Assignment3`):** The main Windows Presentation Foundation (WPF) application where users can select cinemas, view available screenings, and purchase tickets. It uses the Entity Framework Core classes to fetch and display data from the SQL database.

## How to Use

### Pre-requisites

- Ensure you have SQL Server installed.
- Adjust the database connection string in the code to match your SQL Server settings.
- CSV files with movie and cinema information are required for the database population tool.

### Steps

1. **Database Population:**
   - Run the `PopulateDatabase` C# program after providing the necessary CSV files.
   - This will populate the SQL database with cinemas, movies, and screenings.

2. **Running the WPF Application:**
   - Open the `Assignment3` project in Visual Studio.
   - Build and run the WPF application.
   - Interact with the GUI to select cinemas, view screenings, and purchase tickets.

## Contributing

Contributions are welcome! Feel free to submit issues or pull requests.

## License

This project is licensed under the [MIT License](https://choosealicense.com/licenses/mit/).
