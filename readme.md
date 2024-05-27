# Degrees of Separation

This project calculates the degrees of separation between two actors/actresses based on their shared movie roles.

## Overview

The program loads data from CSV files and finds the shortest path of co-starring movie relationships between two given actors. It uses breadth-first search (BFS) to ensure the shortest path is found.

## File Structure

- `degrees.py`: Main script to run the program.
- `util.py`: Contains the `Node`, `QueueFrontier` classes, and additional utility functions.
- `people.csv`: CSV file containing people data.
- `movies.csv`: CSV file containing movies data.
- `stars.csv`: CSV file containing the relationships between people and movies.

## CSV Data Format

### `people.csv`
- `id`: Unique identifier for the person.
- `name`: Name of the person.
- `birth`: Birth year of the person.

### `movies.csv`
- `id`: Unique identifier for the movie.
- `title`: Title of the movie.
- `year`: Release year of the movie.

### `stars.csv`
- `person_id`: ID of the person.
- `movie_id`: ID of the movie.

## How to Run

1. Ensure you have Python installed on your system.
2. Place the `degrees.py` and `util.py` files in the same directory as your data files (`people.csv`, `movies.csv`, `stars.csv`).
3. Open a terminal and navigate to the directory containing these files.
4. Run the following command:

```bash
python degrees.py [directory]

