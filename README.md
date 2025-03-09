## 🌟 Project Overview

**Problem Statement**:  
This project addresses the challenge of maximizing revenue for a renewable energy company that operates a 50 MW utility-scale solar PV system alongside a 10 MW/40 MWh Lithium-ion battery storage system. The goal is to determine the optimal strategy—when to charge, discharge, or purchase grid electricity—based on 15-minute interval electricity prices and simulated solar PV output over a 24-hour period.

Inspired by a complex JuMP (Julia for Mathematical Programming) model originally developed in Julia, this Python implementation demonstrates how to apply algebraic programming techniques to real-world energy management.

## 🔍 Detailed Steps

1. **Step 1: Import Libraries and Modules**  
   Import essential Python libraries such as NumPy, Pandas, and an optimization solver (e.g., Pyomo or CVXPY) that are necessary for building and solving the model.

2. **Step 2: Load Data**  
   Load time series data for electricity prices (15-minute intervals from ERCOT) and simulated solar PV output (sourced from Renewables.Ninja) from CSV files.

3. **Step 3: Data Preprocessing**  
   Clean and format the loaded data. This step includes handling missing values, aligning time indices, and ensuring that both datasets are consistent for further analysis.

4. **Step 4: Define Model Parameters**  
   Establish key parameters such as:
   - Solar PV capacity: 50 MW  
   - Battery power: 10 MW  
   - Battery energy storage: 40 MWh  
   - Other operational constraints  
   These parameters set the boundaries for the optimization model.

5. **Step 5: Define Decision Variables**  
   Define the decision variables that represent the actions to be taken, including:
   - The amount of solar power utilized
   - Battery charging and discharging levels
   - Power transactions with the grid

6. **Step 6: Formulate the Objective Function**  
   Develop an objective function that aims to maximize revenue. This function accounts for the varying electricity prices and the costs/benefits of charging, discharging, or buying grid power over the 24-hour period.

7. **Step 7: Define Constraints**  
   Impose realistic operational constraints such as:
   - Power balance between generation, storage, and grid transactions
   - Battery storage capacity limits
   - Inverter capacity and grid connection restrictions

8. **Step 8: Construct the Optimization Model**  
   Integrate the objective function and constraints into a comprehensive optimization model using an algebraic programming framework.

9. **Step 9: Solve the Optimization Problem**  
   Utilize an optimization solver to compute the optimal operational strategy. This step determines the best schedule for battery charging, discharging, and grid interactions.

10. **Step 10: Analyze the Results**  
    Post-process the solver output to extract key performance metrics. Evaluate revenue outcomes and the feasibility of the operational plan based on the model’s recommendations.

11. **Step 11: Visualization and Reporting**  
    Visualize the results using graphs and charts to illustrate the optimal schedule and performance metrics. Compile a final report summarizing insights and potential areas for further improvement.

## ⚙️ How to Run the Project

1. **Clone the Repository**:
   
   git clone https://github.com/egetamci/SolarBatteryOptimization
   
2. **Navigate to the Project Directory**:
   
   cd SolarBatteryOptimization

3. **Launch the Jupyter Notebook**:
   
   Jupyter notebook main.ipynb
4. **Execute the Notebook Cells**:  
Follow the instructions within `main.ipynb` to load the data, solve the optimization problem, and analyze the results.

## 📦 Requirements

- Python 3.7 or higher
- Jupyter Notebook
- Required libraries: NumPy, Pandas, and an optimization solver (e.g., Pyomo or CVXPY)  
Install dependencies using:

## 🤝 Contributing

Contributions are welcome! If you have suggestions or improvements, please open an issue or submit a pull request.

## 📄 License

This project is licensed under the MIT License.

## 🙏 Acknowledgments

- **Data Sources**: ERCOT electricity market data and simulated solar PV output from Renewables.Ninja.
- **Inspiration**: This project is inspired by a complex JuMP model initially implemented in Julia.


   

   
