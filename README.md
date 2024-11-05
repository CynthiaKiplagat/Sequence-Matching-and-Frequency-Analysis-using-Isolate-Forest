# Sequence Matching and Frequency Analysis combined with Isolation Forest
## Introduction
While working in the financial sector i noticed the importance of patterns and frequency to be able to detect fraud patterns.
### Objective
Detect anomalies based on frequency and sequence variations using Isolation Forest.
### Method 
Use sequence matching techniques and frequency analysis to identify duplicated or patterned transactions.
#### Import Libraries
![Alt Text](https://github.com/CynthiaKiplagat/Sequence-Matching-and-Frequency-Analysis-using-Isolate-Forest/blob/main/Libraries.PNG)
### Load and prepare the data

![Alt Text](https://github.com/CynthiaKiplagat/Sequence-Matching-and-Frequency-Analysis-using-Isolate-Forest/blob/main/Load%20and%20Prepare%20Data.PNG)

After loading the dataset, I performed a thorough check for any missing values and ensured that each column had the correct data type, making necessary adjustments to maintain data integrity and readiness for analysis
### Feature Engineering
For features i decided to split my transaction datetime column to day of the week,month and hour to capture daily,monthly and hourly patterns.

![Alt Text](https://github.com/CynthiaKiplagat/Sequence-Matching-and-Frequency-Analysis-using-Isolate-Forest/blob/main/Feature%20Engineering.PNG)
### Frequency and Sequencing
For additional context I am calculating each accounts daily frequency and rounding the amount to a multiple of 10 to create a sequence to be able to be able to identify repeated sequences.

![Alt Text](https://github.com/CynthiaKiplagat/Sequence-Matching-and-Frequency-Analysis-using-Isolate-Forest/blob/main/Frequency.PNG)

A normal account usually doesnot have more than 5 withdrawal transactions in a day so we set it as our threshold.

![Alt Text](https://github.com/CynthiaKiplagat/Sequence-Matching-and-Frequency-Analysis-using-Isolate-Forest/blob/main/Anomalies%20sequence.PNG)

### Feature Selection
Use key features from daily frequency withdrawn amount and amount rounded for the sequence.
![Alt Text](https://github.com/CynthiaKiplagat/Sequence-Matching-and-Frequency-Analysis-using-Isolate-Forest/blob/main/Feature%20Selection.PNG)

### Model Initiation and visualisation
Fit and training the model to detect anomalies based on frequencies and patterns.
![Alt Text](https://github.com/CynthiaKiplagat/Sequence-Matching-and-Frequency-Analysis-using-Isolate-Forest/blob/main/Model%20Initialisation.PNG)

Visualise the data to be able to see the anomalies







