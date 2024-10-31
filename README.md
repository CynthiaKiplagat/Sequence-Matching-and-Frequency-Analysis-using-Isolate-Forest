# Advanced Transaction Anomaly Detection in Financial Data Using Isolation Forest
## Introduction
Building on my experience in the financial sector, I am delving into advanced analytics with a focus on Isolation Forest to deepen my expertise in transaction anomaly detection.
### Purpose
To detect repetitive sequences in mobile transactions, which can indicate fraud patterns.
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
For additional context I am calculating each accounts daily frequency and rounding the amiunt to a multiple of 10 to create a sequence to be able to be able to under their behaviour.
![Alt Text](https://github.com/CynthiaKiplagat/Sequence-Matching-and-Frequency-Analysis-using-Isolate-Forest/blob/main/Frequency.PNG)

A normal account usually doesnot have more than 5 withdrawal transactions in a day so we set it as our threshold.

![Alt Text](https://github.com/CynthiaKiplagat/Sequence-Matching-and-Frequency-Analysis-using-Isolate-Forest/blob/main/Anomalies%20sequence.PNG)



