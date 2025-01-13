# PERT Analysis Tool for Dynamic Scheduling

## Overview
This project implements a **PERT (Program Evaluation and Review Technique)** tool for dynamic scheduling. It allows users to input project activities with their optimistic, most likely, and pessimistic time estimates. The tool calculates expected times, standard deviations, and identifies the critical path. Additionally, it computes the probability of completing the project within a given time frame using the Z-score from the normal distribution.

## Features
- **Input Activities**: Input project activities with optimistic, most likely, and pessimistic time estimates.
- **Expected Time & Standard Deviation Calculation**: Calculates expected time and standard deviation for each activity using the PERT formula.
- **Critical Path Calculation**: Identifies the critical path in the project network.
- **Probability of Completion**: Calculates the probability of completing the project within a specified duration.
- **Z-Score and Tabulated Probability**: Computes the Z-score and provides the cumulative probability from the normal distribution.
- **Graphical Visualization**: Visualizes the project network and highlights the critical path.
- **Interactive GUI**: Built using **Tkinter** for an intuitive user interface.

## Prerequisites
Make sure you have the following installed:
- Python 3.x
- Required Python libraries:
  ```bash
  pip install networkx matplotlib scipy pillow

## How to Run
1. Run the `Project lpt.py` script:
   ```bash
   python Project lpt.py
   ```
2. Use the GUI to input the following details for each project activity:
   - **Activity (start-end):** Specify the activity (e.g.,`1-2`).
   - **Optimistic Time (O):** Enter the optimistic time estimate.
   - **Most Likely Time (M):** Enter the most likely time estimate.
   - **Pessimistic Time (P):** Enter the pessimistic time estimate.
   - **Desired Project Duration:** Enter the desired project duration for probability calculation.

3. After entering all activities, click **Done** to view the results, including:
   - **Critical Path**
   - **Total Duration**
   - **Probability of Completion**
   - **Z-Score**
   - **Tabulated Probability**
   - **Normal Distribution Curve Visualization**

## Example
1. Enter the following activities:
   - **Activity**:`1-2`,**Optimistic**:`1`,**Most Likely**:`1`,**Pessimistic**:`7`
   - **Activity**:`1-3`,**Optimistic**:`1`,**Most Likely**:`4`,**Pessimistic**:`7`
     ![image](https://github.com/user-attachments/assets/45b48237-8c32-4731-bc09-2c7545745e47)

2. Click **Done** to calculate and view the results:
   - **Critical Path**:`1 -> 3 -> 5 -> 6`
   - **Total Duration**:`17`days
   - **Probability of Completion**:`74.54%`
   - **Z-Score**:`0.66`
   - **Tabulated Probability**:`0.7454`
  
## Screenshots
### Main Window
![image](https://github.com/user-attachments/assets/b9fcbedc-2e0e-4eb9-abe0-be5f403a102f)

### Project Network Diagram with the critical path highlighted
![image](https://github.com/user-attachments/assets/fa39aeb0-17c0-4c8b-9ce1-d4cea48a5f17)

### Shaded Region under Z-Score
![image](https://github.com/user-attachments/assets/5166fa26-f7f2-4ae4-8565-44f899fe7b49)

