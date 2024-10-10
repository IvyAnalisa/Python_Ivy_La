# Python_Advanced_Course 2024
# Projects in this course has been completed by assigments in everyweek which my teach gave me.
Certainly! Here’s a sample README file for the simulation project you’ve worked on. It includes sections about the project, how to set it up, and how to run it, along with a brief explanation of the main features.

---

# **Pandemic Simulation Project** (from uppgift 3,4,5)

## **Overview**

This project simulates the spread of a virus in a village community over time. The simulation models the infection, recovery, death, and vaccination processes, allowing users to track the pandemic's progression within a population. The data is collected and visualized through various plots to understand how the virus affects the population.

The simulation includes features such as:
- Simulating individual person behavior (infection, recovery, death, and vaccination).
- Tracking key metrics like the number of sick, recovered, deceased, vaccinated, and susceptible individuals.
- Visualizing the data using different types of plots (line charts, bar charts, and subplots).

## **Features**
1. **Simulation of virus spread**:
   - Each person can get sick, recover, die, or become vaccinated.
   - Infection spreads based on random encounters and probabilities.
   
2. **Data tracking**:
   - Number of sick, recovered, deceased, vaccinated, and immune individuals tracked for each day.

3. **Plotting**:
   - **Line plots**: A comprehensive graph showing the trends of the sick, recovered, deceased, vaccinated, immune, and susceptible populations over time.
   - **Bar plots**: A bar chart that shows the number of sick individuals each day.
   - **Subplots**: Two side-by-side plots displaying trends for the sick and recovered populations separately.

## **Technologies Used**

- **Python**: The core programming language used for simulation and data manipulation.
- **Pandas**: For handling and manipulating the simulation data.
- **Matplotlib**: For creating visualizations (line plots, bar plots, and subplots).
- **Numpy**: For numerical operations (e.g., linspace to generate axis values).

## **How the Simulation Works**
Each day, the simulation tracks the status of every person in the population. The individual statuses include:
- **Sick**: The person is infected with the virus.
- **Recovered**: The person was sick and recovered from the virus.
- **Deceased**: The person did not recover and passed away due to the virus.
- **Vaccinated**: The person received a vaccine, which protects them from getting infected.

The simulation runs until no one is sick anymore, at which point it terminates.

## **Project Structure**

- `Person`: A class representing an individual person with attributes and behaviors for infection, recovery, and vaccination.
- `Village`: A class that represents the village, managing the population and simulation over multiple days.
- **Plots**:
  - Line plot of population statistics.
  - Bar plot of the sick population.
  - Side-by-side subplots for sick and recovered population trends.

## **Getting Started**

### **Prerequisites**
To run this project, you will need:
- Python 3.x installed.
- Required libraries: `pandas`, `matplotlib`, `numpy`.

You can install the necessary dependencies with the following command:

```bash
pip install pandas matplotlib numpy
```

### **Running the Project**

1. **Clone the Repository**:
   ```bash
  (https://github.com/IvyAnalisa/Python_Ivy_La.git)
   cd pandemic-simulation
   ```

2. **Run the Simulation**:
   The main Python script simulates the village's population during a pandemic and generates visualizations.
   To run the simulation:
   
   ```bash
   python your_script_name.py
   ```

   The simulation will:
   - Generate a CSV file (`my_ass5_dataset.csv`) containing the daily statistics.
   - Display a line plot showing the progression of the virus over time.
   - Display a bar chart showing the number of sick individuals each day.
   - Show two side-by-side plots: one for the sick population and one for the recovered population.

### **Visualizations Generated**

1. **Line Plot**: Shows the trends of sick, recovered, deceased, vaccinated, immune, and susceptible individuals over time.

2. **Bar Plot**: Shows the number of sick individuals per day.

3. **Subplots**: 
   - One plot shows the sick population over time.
   - The other plot shows the recovered population over time.

### **Main Functions**

- `start_simulation()`: Controls the progression of days in the village and records data for each day.
- `plot_data()`: Plots the trends of various population categories over time using a line chart.
- `bar_plot()`: Generates a bar chart for the number of sick people each day.
- `mult_plots()`: Displays two side-by-side plots for the sick and recovered populations.

## **Customization**
- You can modify parameters like the population size, probabilities for infection, recovery, and death, as well as vaccination rates in the `Person` and `Village` classes to simulate different scenarios.

## **Future Enhancements**
- Add more detailed tracking of individual recovery time or additional visualizations such as pie charts for distribution across categories (e.g., immune vs. susceptible).
- Incorporate more advanced simulation features like immunity after recovery or reinfection scenarios.
  
