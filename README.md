# Medical-Insurance-Project
A Personal Project in Data and Programming Foundations for AI


Medical Insurance Cost Estimator

Overview

This project is a simple Python-based application that estimates health insurance costs using personal attributes such as age, BMI, smoking status, and number of dependents.

It also includes functionality to compare insurance costs between individuals.

The goal of this project is to demonstrate core programming concepts such as:

Function design
Data handling
Basic mathematical modeling
Clean and readable code practices

 Features
 Estimate insurance cost using a mathematical formula
 Compare costs between two individuals
 Clear and reusable function design
 Readable output messages
Insurance Cost Model

The estimated insurance cost is calculated using the following formula:

cost = 250 * age 
     - 128 * sex 
     + 370 * bmi 
     + 425 * children 
     + 24000 * smoker 
     - 12500
Parameters:
age (int): Age of the individual
sex (int): 0 = female, 1 = male
bmi (float): Body Mass Index
children (int): Number of dependents
smoker (int): 0 = non-smoker, 1 = smoker

Usage
Run the script:
python main.py
Example:
cost, message = calculate_insurance_cost("Maria", 28, 0, 26.2, 0, 3)
print(message)
Compare two individuals:
diff, msg = insurance_cost_difference(cost1, cost2)
print(msg)
 Example Output
Maria's estimated insurance cost is 9490.00 dollars.
Omar's estimated insurance cost is 5464.00 dollars.
The difference in insurance cost is 4026.00 dollars.

Limitations
This is a simplified model and does not reflect real-world insurance pricing
No input validation is implemented
The dataset and formula are static

Ethical Considerations

The model includes variables such as sex, which can influence the output.
In real-world applications, the use of sensitive attributes must comply with legal and ethical standards.

This project is for educational purposes only.

Requirements
Python 3.x
No external libraries required


 Future Improvements

Add input validation
Build a user interface (CLI or web app)
Use real datasets for more accurate predictions
Visualize results using charts