# Degrees of Separation (CS50 AI Project)

This project is part of the CS50 AI curriculum and implements the Degrees of Separation problem, similar to the "Six Degrees of Kevin Bacon" game. The goal of the project is to find the shortest path between two actors based on their shared movie appearances.

## Project Overview

The Degrees of Separation program uses a graph-based approach to find the shortest connection between two actors. It loads data from CSV files containing information about people (actors), movies, and the relationships between them. Given two actor names, it finds the shortest path between them in terms of co-starring in movies.

## Project Structure

degrees/
    large/                  - Large dataset for Degrees of Separation
    small/                  - Small dataset for Degrees of Separation
    degrees.py              - Main program for Degrees of Separation
    util.py                 - Helper classes (Node, StackFrontier, QueueFrontier)
README.md                   - Project readme file
requirements.txt            - Required Python dependencies

## Data

The project uses two datasets (large and small) stored in CSV format:
- people.csv: Information about actors (ID, name, birth year).
- movies.csv: Information about movies (ID, title, year).
- stars.csv: Mapping of actors to movies they've starred in.

## Setup

1. Clone the repository:
   git clone https://github.com/yourusername/degrees-of-separation.git
   cd degrees-of-separation

2. Install dependencies:
   Ensure you have Python 3 installed, then install the required dependencies:
   pip install -r requirements.txt

3. Download/Prepare Data:
   The project includes small and large datasets in the degrees/ directory.

## Usage

To find the shortest connection between two actors:
   python degrees/degrees.py degrees/large

You will be prompted to enter two actor names, and the program will find the shortest path between them based on their movie co-stars.

## Example:
Name: Tom Hanks
Name: Kevin Bacon

If the actors are connected, the program will display the degrees of separation and the movies connecting them.
