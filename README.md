# Smart Washing Machine (Advanced)–Fuzzy Logic System

## Project Overview

This project implements an **Advanced Smart Washing Machine using Fuzzy Logic** in Python.  
The system intelligently determines the appropriate **washing intensity** based on multiple input conditions using the **Mamdani Fuzzy Inference System**.

Unlike traditional binary systems, this project simulates **human-like decision making** by handling uncertainty and overlapping conditions through fuzzy logic.


# Objectives

The main objectives of this project are to:

- Apply **Artificial Intelligence and Fuzzy Logic concepts**
- Design a **Mamdani-based Fuzzy Inference System**
- Implement:
  - Fuzzification
  - Rule Evaluation
  - Aggregation
  - Defuzzification
- Generate intelligent washing decisions automatically
- Visualize fuzzy membership functions graphically


# Input Variables

## 1. Cloth Type

| Value | Type |
|------|------|
| 1 | Delicate |
| 2 | Normal |
| 3 | Heavy |


## 2. Load Size (kg)

Range: **0 – 15 kg**

| Category | Range |
|------|------|
| Small | 0 – 5 |
| Medium | 5 – 10 |
| Large | 10 – 15 |


## 3. Dirtiness Level

Range: **0 – 10**

| Category | Range |
|------|------|
| Low | 0 – 3 |
| Medium | 3 – 7 |
| High | 7 – 10 |


## 4. Water Hardness (ppm)

Range: **0 – 500 ppm**

| Category | Range |
|------|------|
| Soft | 0 – 166 |
| Normal | 166 – 333 |
| Hard | 333 – 500 |

# Output Variable

## Washing Intensity (%)

| Category | Meaning |
|------|------|
| Gentle | Low detergent and low agitation |
| Normal | Moderate washing |
| Strong | High detergent and strong agitation |

Output Range: **0 – 100%**

# Technologies Used

- Python
- NumPy
- Scikit-Fuzzy
- Matplotlib
- Google Colab

# Fuzzy Logic Technique Used

## Mamdani Fuzzy Inference System

The project follows the standard fuzzy logic workflow:

1. Crisp Input Collection
2. Fuzzification
3. Rule Evaluation
4. Aggregation
5. Defuzzification
6. Crisp Output Generation

# Membership Functions

The project uses **Triangular Membership Functions (trimf)** for both input and output variables.

Membership functions are used to represent linguistic values such as:

- Low
- Medium
- High
- Gentle
- Normal
- Strong


# Fuzzy Rules

The system uses rule-based decision making.

## Rule 1
IF Cloth = Heavy AND Load = Large AND Dirtiness = High  
THEN Washing Intensity = Strong

## Rule 2
IF Cloth = Delicate AND Water Hardness = Hard  
THEN Washing Intensity = Gentle

## Rule 3
IF Cloth = Normal AND Load = Medium AND Dirtiness = Medium  
THEN Washing Intensity = Normal

## Rule 4
IF Cloth = Normal AND Load = Large AND Dirtiness = High  
THEN Washing Intensity = Strong

## Rule 5
IF Cloth = Delicate AND Dirtiness = Low  
THEN Washing Intensity = Gentle

## Rule 6
IF Cloth = Heavy AND Dirtiness = Medium  
THEN Washing Intensity = Normal

## Rule 7
IF Cloth = Normal AND Water Hardness = Hard  
THEN Washing Intensity = Normal


# Defuzzification Method

The system uses the:

## Centroid Method (Center of Gravity)

This method converts the aggregated fuzzy output into a final crisp washing intensity percentage.


# Features of the Project

- Advanced fuzzy inference system
- Intelligent washing decision system
- User input validation
- Dynamic console interaction
- Crisp input display
- Fuzzification result calculation
- Rule inference evaluation
- Aggregation process
- Centroid defuzzification
- Graph visualization
- Membership function plotting
- Output classification label generation

# Graphs Generated

The system generates graphical membership functions for:

1. Cloth Type
2. Load Size
3. Dirtiness Level
4. Water Hardness
5. Washing Intensity Output


# Example Input

Cloth Type = 3
Load Size = 13 kg
Dirtiness = 1
Water Hardness = 131 ppm

# Example Output
Washing Intensity = 50.0000%
Washing Label = NORMAL

# Project Workflow

User Input
     ↓
Fuzzification
     ↓
Rule Evaluation
     ↓
Aggregation
     ↓
Defuzzification
     ↓
Final Crisp Output

# Academic Concepts Covered

* Artificial Intelligence
* Fuzzy Logic
* Mamdani Inference System
* Membership Functions
* Rule-Based Systems
* Defuzzification
* Intelligent Automation
* Decision-Making Systems

# Installation

Install required libraries before running the project:
python
pip install scikit-fuzzy matplotlib numpy
(!pip install scikit-fuzzy)

# How to Run

1. Open the notebook in Google Colab or Jupyter Notebook
2. Install required libraries
3. Run all cells
4. Enter input values when prompted
5. Observe fuzzy outputs and generated graphs

# Conclusion

This project successfully demonstrates how fuzzy logic can be applied in a real-world smart washing machine system.

The fuzzy inference system intelligently determines washing intensity based on multiple uncertain and overlapping conditions, providing more flexible and human-like decision making compared to traditional systems.

The project also demonstrates practical implementation of:

* Fuzzy Membership Functions
* Mamdani Inference System
* Centroid Defuzzification
* Rule-Based AI Systems
* Graphical Fuzzy Analysis
  
# Author

-Name:Jubaida Begum
-Department:CSE
-Institution: Leading University, Sylhet
-Project Title:Smart Washing Machine(Advanced)–Fuzzy Logic System
