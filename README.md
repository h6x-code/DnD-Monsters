# D&D Monster Threat Analysis & CR Estimator
This project explores statistical and machine learning techniques to analyze and predict Challenge Ratings (CR) of monsters from Dungeons &amp; Dragons 5e.

## Overview

Using a dataset of official D&D monsters, the project performs:

- Exploratory Data Analysis on monster stats (HP, AC, STR–CHA, etc.)
- Feature engineering to derive a custom Threat Score
- CR prediction via Random Forest Regression
- An interactive CR estimator built with ipywidgets and Voila

---

## Features

- Cleaned and transformed monster dataset
- Custom threat score formula:  
  `threat_score = avg_stat * (hp + ac) * (1.25 if legendary)`
- Visual insights: stat distributions by CR, type, and legendary status
- CR prediction model using `scikit-learn`
- Interactive UI for estimating CR based on monster stats

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/h6x-code/DnD-Monsters.git
   cd DnD-Monsters

2. Launch Jupyter or Voila:
   ```bash
   jupyter notebook
   # or
   voila "Monsters of D&D - Statistical Insights.ipynb"

## Files
"Monsters of D&D - Statistical Insights.ipynb" – annotated analysis with explanations

dnd_monsters.csv - D&D monster CSV file

## Example Use
Use the interactive estimator to test homebrew monster builds. Input HP, AC, stats, and legendary status, and get:

- A predicted CR
- A threat score
- A comparison to average monsters at that CR
- A threat score vs CR plot

## License
MIT License. Feel free to fork, adapt, and extend the project.

## Credits
Project by McKinley West. Built with Python, Pandas, Seaborn, Scikit-learn, and Jupyter Widgets.
Original Dataset from mrpantherson on Kaggle (https://www.kaggle.com/datasets/mrpantherson/dnd-5e-monsters).
