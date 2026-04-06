# Databases-Project: HotelDB Enterprise
A professional Full-Stack Management System that automates hotel operations using a centralized SQL Server database and a Python Streamlit dashboard.

#1. System Architecture
   Database (SQL Server): 6 normalized tables (Guest, Room, RoomType, Reservation, Payment, Service) ensuring data integrity.

   Interface (Python): A multi-page Streamlit web app providing staff with tools for bookings and management.

   Middleware: pyodbc utilizing the modern ODBC Driver 17 for high-speed, secure data communication.

#2. Advanced SQL Implementation
   Stored Procedures: Used MakeReservation and CheckAvailability to handle complex business logic (pricing, date validation) directly on the server.

   Triggers: Automated room status updates (Available ↔ Occupied) based on reservation changes to eliminate manual errors.

    Views: Real-time reporting via MonthlyOccupancy and RevenueByRoomType for instant business analytics.

    Indexes: Optimized queries using non-clustered indexes on Email, Status, and Date columns for faster search results.

#3. Key Features
    Conflict Prevention: Logic-level checks to prevent double-booking of rooms.

    Guest Management: Full registration system with document tracking.

    Live Dashboard: Visual metrics for total revenue and occupancy trends.

    Automated Billing: Calculation of stay totals and cancellation fees handled by backend procedures.

#4. Presentation Summary
"This project demonstrates a production-ready DBMS where all critical business rules are enforced by the database itself, ensuring reliability regardless of the frontend used. It bridges the gap between raw data and executive decision-making."
