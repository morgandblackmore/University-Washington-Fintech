# 14_ml_algorithmic_trading
Use ML models to evaluate algorithmic trading strategy

---

## Technologies  
Uses Jupyter Lab, Python, Scikitlearn, SVC, AdaBoost.  

---  

## Installation Guide  
1. Download this repo.  
2. Install [Jupyter Lab](https://jupyterlab.readthedocs.io/en/stable/getting_started/installation.html) if you don't already have it.  
3. Open machine_learning_trading_bot.ipynb in Jupyter Lab.  

---  

## Usage  
This project consists of 4 Sections:  
1. Generating a baseline model (consisting of 7 labeled steps)
2. Tuning baseline by changing the time period  
3. Tuning the baseline by changing the moving average period
4. Generating a new model using a different ML algorithm


You can run all cells consecutively up until the start of Section 3. In order to avoid repeating large sections of code, you will need to:  
1. Run the first part of Section 3  
2. Go to Section 1 and rerun the cells for Step 3  
3. Go back to Section 3 and finish running the remaining celuls.  
This reloads the baseline model with the new parameters.  
  
To run Section 4, you will need to rerun Section 1 (resetting the baseline training parameters) and then run Section 4.  
  
Alternatively, you could run Sections 1,2, and 4 first, then follow the steps for Section 3.
 
---  

## Results  
Baseline: 
![Baseline Report](/Starter_Code/Resources/baseline_report.png)
![Baseline Graph](/Starter_Code/Resources/baseline_returns.png)

Time period / size of dataset:  
![Time Adjusted Report](/Starter_Code/Resources/6mo_report.png)  
![Time Adjusted Graph](/Starter_Code/Resources/6mo_returns.png)  
  
SMA adjusted:  
![SMA Adjusted Report](/Starter_Code/Resources/adjusted_sma_report.png)  
![SMA Adjusted Graph](/Starter_Code/Resources/adjusted_sma_returns.png)  
  
AdaBoost:  
![AdaBoost Report](/Starter_Code/Resources/adaboost_report.png)  
![AdaBoost Graph](/Starter_Code/Resources/adaboost_returns.png)
  


---  

## Contributors  
Base code provided as class materials but skillfully updated by Morgan Blackmore.  

---  

## License  
Code provided under [MIT](https://mit-license.org/) license.
