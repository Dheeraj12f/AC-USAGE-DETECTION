----Air Conditioner Usage Detection from Electrical Current Data-----


Project Overview
This project analyzes household electrical data to identify when an Air Conditioner (AC) is operating. The dataset contains measurements of voltage, current, and timestamp from a smart energy monitoring system.
By analyzing the current consumption patterns, we detect periods when the AC is running. The AC typically draws significantly higher current than other household appliances, which allows it to be identified using data analysis techniques.
This project demonstrates basic time-series analysis, data preprocessing, and energy consumption analysis using Python.

-------------------------------Dataset Description-----------------------
The dataset contains the following columns:
             ---Column
             ---Description
             ---device_timestamp
Timestamp of measurement (in milliseconds)
voltage
Electrical voltage reading (Volts)
current
Total current consumption (Amperes)
The current value represents the total load of all appliances connected to the household electrical system.
--------------------------------Project Objective-------------------------
The goal of this project is to:
Analyze electrical current data
Identify patterns associated with AC operation
Separate AC usage from other appliances
Visualize energy consumption trends using graphs


--------------------Methodology----------------
1. Data Loading
2. Timestamp Conversion
3. Signal Smoothing
4. AC Detection
5. Power Consumption Calculation
Power consumption is estimated using the formula: Power = Voltage * Current

--------------------Visualizations-------------
The project generates several graphs to analyze electricity usage:
Total Current Consumption Over Time
Smoothed Current Signal
Detected AC Usage
Power Consumption Graph
These graphs help identify AC startup spikes, running patterns, and compressor cycles.


-------------------Key Observations--------------
Normal household appliances consume very low current (0.02–2 A).
Air conditioner operation creates large current spikes (10–14 A).
Occasionally, the AC shows startup surges up to ~25 A, which correspond to compressor inrush current.
Power consumption during AC operation typically ranges between 2500W and 3200W.


----------------------Technologies Used---------------
Python
Pandas
Matplotlib
Jupyter Notebook / Google Colab

-------------------NEXT STEP-----------
Train ML model
Testing and slecting best model by checking accuracy
saving model 
build simple UI using streamlit

