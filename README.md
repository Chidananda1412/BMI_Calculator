

# BMI Calculator

This project is a BMI (Body Mass Index) calculator with a graphical user interface (GUI) built using Tkinter. The application allows users to input their weight and height, calculate their BMI, and categorize it. Additionally, it stores the data in an SQLite database and provides functionality to plot the BMI trend over time using Matplotlib.

## Features

- Calculate BMI using weight and height.
- Classify BMI into categories: Underweight, Normal weight, Overweight, and Obese.
- Display the calculated BMI and its category.
- Store BMI data in an SQLite database.
- Plot the BMI trend over time using stored data.

## Prerequisites

- Python 3.x
- Tkinter (usually comes pre-installed with Python)
- SQLite3 (usually comes pre-installed with Python)
- Matplotlib

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/file_name.git
   cd Address_to_the_folder
   ```

2. **Install the required Python libraries:**
   ```bash
   pip install matplotlib
   ```

## Usage

1. **Run the application:**
   ```bash
   python bmi_calculator.py
   ```

2. **Using the GUI:**
   - Enter your weight in kilograms.
   - Enter your height in meters.
   - Click the "Calculate BMI" button to calculate and display your BMI and its category.
   - Click the "View BMI Trend" button to plot the BMI trend using stored data.
   - Click the "Quit" button to exit the application.

## Project Structure

- **bmi_calculator.py**: The main script containing the BMI calculator functionality and GUI code.

## Functions

### `calculate_bmi(weight, height)`

Calculates BMI using the given weight and height.

**Parameters:**
- `weight` (float): Weight in kilograms.
- `height` (float): Height in meters.

**Returns:**
- `float`: Calculated BMI.

### `classify_bmi(bmi)`

Classifies the given BMI into categories.

**Parameters:**
- `bmi` (float): Calculated BMI.

**Returns:**
- `str`: BMI category.

### `calculate_and_display()`

Calculates BMI, displays the result, and saves the data to the database.

### `create_table()`

Creates the database table if it doesn't exist.

### `save_data(weight, height, bmi)`

Saves the BMI data to the database.

**Parameters:**
- `weight` (float): Weight in kilograms.
- `height` (float): Height in meters.
- `bmi` (float): Calculated BMI.

### `plot_bmi_trend()`

Plots the BMI trend from the stored data.

## Database

The application uses an SQLite database (`bmi_data.db`) to store BMI records. The database contains a single table `bmi_records` with the following columns:
- `id` (INTEGER PRIMARY KEY): Unique identifier for each record.
- `weight` (REAL): Weight in kilograms.
- `height` (REAL): Height in meters.
- `bmi` (REAL): Calculated BMI.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request or open an issue to discuss improvements or fixes.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.

## Acknowledgments

- The Tkinter library for the GUI.
- The Matplotlib library for plotting.
- The SQLite database for data storage.

