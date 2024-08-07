# CapstoneArchery - Data Analysis Project

## Overview

The project is my capstone project for CODE:You. The purpose of this capstone project is to create a report based on shot execution data collected during 3D archery events.  This report can then be used by the archer to evaluate their performance and identify trends in their shot execution which can then be corrected / addressed for future tournaments.  The scope of this project is to create a report containing different data elements collected in the field using a Survey123 mobile application.  Trends will be identified through a list of predefined criteria and presented within the report for the archer to then evaluate. 

## Data

Data was created and collected using esri's ArcGIS Online platform in support of this project. Three distinct layers will be referenced for this project:<br>
1.  A lookup table was created containing the various 3D target animals along with information on the color, size, name, and target pattern.<br> 
2.  A Survey123 was created to collect shoot conditions for each tournament.  Data was collected to capture the shoot name, shoot location (indoor or outdoor), shoes (minimal, hiking boots, sandals, gym shoes), temperature, weather conditions present (sunny, cloudy, humid, windy, foggy, light rain, heavy rain, stormy), and personal conditions (well rested, tired, sick, sore, hungry, full).<br>
3.  A Survey123 was created to collect several details for each shot on the individual target and appearance (animal, range, position, elevation, lighting), shot execution (confidence, release details, execution details), and placement (score, aim placement, actual arrow impact).

### Project Structure
---

The project is organized as follows:

- **Data Exploration:** Jupyter notebooks or scripts to explore the dataset.

- **Analysis:** Using Python with the Pandas package to clean the data.

- **Visualizations :** Using Dash and Plotly to visualize my findings. 


## Features Utilized for the project

  | Feature        | Description                           |
  |----------------|---------------------------------------|
  | Read TWO data files| Used 3 layers created within ArcGIS online and referenced through dataframes          |
  | Clean your data and perform a pandas merge with your two data sets, then calculate some new values based on the new data set.      | Pulled my data into a data frame, cleaned my data and merged them with pandas merge to a new dataframe. Added and calculated fields in the new dataframe for facilitating graphic productions |
  | Make 3 matplotlib or seaborn (or another plotting library) visualizations to display your data. | Made various plots to display findings. |
  | Best Practices:  Utilize a virtual environment with a requirements file, README file, and pseudocode.      | Created a VENV for the project, populated the README file, used pseudocode and markdown cells to explain the code.  |


## Getting Started

To run this project, follow these steps:

1. Clone the repository: `git clone https://github.com/ecbartee/CapstoneArchery.git`
2. Create a virtual environment to install the needed modules to. 
3. Install the necessary dependencies: `pip install -r requirements.txt` - if this fails review the requirements text file and manually install the required modules if needed.
4. Explore the ArcheryCapstone.ipynb Jupyter notebook within the Python folder

## Dependencies

The following Modules are used in this project:
- ipykernel
- arcgis
- pandas
- pandasql
- os
- requests
- IPython
- plotly
- ipywidgets
- dash

###  Virtual Environment Instructions
---
1. After you have cloned the repo to your machine, navigate to the project 
folder in GitBash/Terminal.
2. Create a virtual environment in the project folder. 
3. Activate the virtual environment.
4. Install the required packages. 
5. When you are done working on your repo, deactivate the virtual environment.

Virtual Environment Commands

| Command | Linux/Mac | GitBash |
|---------|-----------|---------|
| Create | `python3 -m venv venv` | `python -m venv venv` |
| Activate | `source venv/bin/activate` | `source venv/Scripts/activate` |
| Install | `pip install -r requirements.txt` | `pip install -r requirements.txt` |
| Deactivate | `deactivate` | `deactivate` |