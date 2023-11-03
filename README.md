## [Project 1: Exploratory Data Analysis - TTC Subway Delay]
### Introduction
![image](https://github.com/anbui-da/TTC-Subway-Delay/assets/58675665/ee54cdf1-fb64-4f80-8360-73642c6fb7bf)

Public transportation systems, including buses, streetcars, and subways, play a crucial role in keeping Toronto moving. However, in recent years, wait times have ballooned. As a commuter keen to better understand the intricacies of Toronto's public transportation network, I embarked on a comprehensive data analysis project focused on TTC Subway delays. With that objective, I conducted exploratory data analysis, time series evaluation, the project unveiled the patterns of TTC Subway delay. he "TTC Suway delay data" is downloaded from the open portal of City of Toronto which includes 19,895 entries and 10 columns which recorded everday incident, capturing crucial features such as the date, time, station, line, codes and the length of delay in minutes.

### Methodology
Leveraging  Python Pandas, Numpy, Matplotlib, Seaborn for data preprocessing and analysis.

### Findings
**1. Univariate analysis:**
  - Min Delay: The majority of delays are quite short, mostly ranging between 0 to around 10 minutes. There are a few delays that extend beyond this range, but they are less frequent.
  - The top 5 delay codes: 
    - SUDP: Disordely Patron
    - PUOPO: Train door monitoring
    - MUATC: ATC project
    - MUPAA: Passenger Assistance Alarm Activated - No Trouble Found
    - SUUT: Unauthorized at Track Level
  - Top stations with most frequent delays:
    - Finch, Eglington and Kennedy are the top stations with the highest frequency of delay.
    - Regarding to Finch station's delay, TUNOA, TUNIP and MUTO were the top 3 codes that had the highest Min Delay.
    
**2. Bivariate analysis:**
  - All the correlation coefficients are very close to zero, suggesting that there is a very weak relationship between these categorical variables ('Day', 'Bound', 'Line', 'Station') and the continuous variable ('Min Delay'). Therefore, it's likely that these variables alone do not have a strong predictive power for the length of delays.
  - Throughout the year 2022, the number of delays showed a downtrend over time by Month. It showed a significant drop in number of delays from Jan to Feb but fluctuated unitl Dec.
  - The number of delays was at peaked on Friday while it is noticeably lower during the weekends (Saturday and Sunday).
  - SUDP, SUUT are the top Codes that had the highest delay in hours.
  - The number of delays is higher during peak hours (from 6AM-8AM and 16PM-18PM) than off-peak hours. This is expected as there are more people travelling during peak hours than off-peak hours.
  - SUDP (disorderly patron) is the top Code which accounted for the highest delays in minutes for each week day.
