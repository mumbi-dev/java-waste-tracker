# GreenTrack Waste Management System

A Java-based console application designed to track household waste submissions, calculate environmental impact scores (GSP), and generate comprehensive system reports. 

This project was built to demonstrate core Object-Oriented Programming (OOP) principles and robust error handling.

## Features
- **Household & Collector Registration:** Manage users and their service areas.
- **Waste Submission:** Log waste items categorized as Plastic, Organic, or Hazardous.
- **Eco-Score Calculation:** Dynamically calculates an impact score based on waste type and weight using polymorphic multipliers.
- **System Reports:** Generates reports showing total waste by category and total environmental impact per household.
- **Input Validation:** Uses custom exceptions and validation services to ensure data integrity.

## Architecture & OOP Principles
- **Inheritance & Polymorphism:** `WasteItem` is an abstract class. `PlasticWaste`, `OrganicWaste`, and `HazardousWaste` extend it, providing their own `getGSPMultiplier()` implementations.
- **Interfaces:** `WasteTrackable` defines the contract for calculating impact scores.
- **Encapsulation:** Models use private fields with public getters/setters.
- **Custom Exceptions:** `InvalidWasteTypeException` and `InvalidWasteWeightException` handle domain-specific errors.
- **Layered Design:** Separated into `model`, `service`, `util`, and `main` packages for clean code organization.

## How to Run
1. Clone the repository.
2. Compile the project using the provided batch script (Windows):
   ```cmd
   compile.bat
