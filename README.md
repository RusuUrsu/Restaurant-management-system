
# Restaurant Reservation App

This .NET application is designed to facilitate restaurant reservations for users and management for restaurant owners. The app uses a SQL database to store and query restaurant and reservation information. It offers two primary user roles: **Client (User)** and **Admin (Restaurant Owner)**, each with unique functionalities. 

## Features

- **User Roles**:
  - **Client**: Allows users to search for restaurants, view available tables by date, and make reservations.
  - **Admin**: Enables restaurant owners to manage restaurant data, add or update restaurant details, and view reservation statistics.

- **Login and Sign-Up**:
  - Secure login and sign-up options with role-based access.
  - Sign up as either a **Client** or an **Admin**.

- **Restaurant Search with Map Integration**:
  - Search for restaurants by name using a database query.
  - Integrated Google Maps search through a web browser control for location-based searches.
  
- **Reservations**:
  - Select a restaurant, date, and view available tables.
  - Reserve a table, with the reservation details stored in the database.
  - Reservations occupy specific tables at specified dates to prevent double-booking.

- **Admin Management Tools**:
  - Add or edit restaurant details in the database.
  - Access restaurant-specific statistics to understand booking trends.

## Getting Started

### Prerequisites

- .NET SDK 5.0 or later
- SQL Server or SQL Express (for database setup)
- Visual Studio or any preferred C# IDE


### Client-Side (User)

1. **Login or Sign-Up**: 
   - New users can register as **Clients**.
   - Returning users can log in with their credentials.

2. **Restaurant Search**:
   - Search by restaurant name: Performs a lookup in the app’s database.
   - Search using Google Maps: Integrated map search for finding nearby restaurants.

3. **Make a Reservation**:
   - Choose a restaurant and specify a date.
   - View available tables for the selected date.
   - Reserve a table, which is then recorded in the database.

### Admin-Side (Restaurant Owner)

1. **Login or Sign-Up**: 
   - New users can register as **Admins**.
   - Returning users can log in with admin credentials.

2. **Restaurant Management**:
   - Add or update restaurant information.
   - View and manage restaurant data stored in the database.

3. **View Statistics**:
   - Access statistics to monitor restaurant performance and booking trends.

## Database Structure

The SQL database includes the following tables:

- **Users**: Stores user data with role-based fields for client and admin types.
- **Restaurants**: Contains information about each restaurant (name, address, etc.).
- **Tables**: Lists available tables for each restaurant and their seating capacities.
- **Reservations**: Stores reservation details, including restaurant ID, table ID, user ID, and date/time.
