# trader-behavior-fear-greed
This project analyzes the relationship between trader behavior and performance and the Crypto Fear & Greed Index. The goal is to understand how different market sentiment regimes (Fear, Neutral, Greed) impact:
a)Trader profitability (PnL)
b)Win rate
c)Trading behavior and directional bias
d)The analysis is performed strictly using the provided datasets, with full validation of column structures and timestamp formats.

📂 Datasets Used
1️⃣ Historical Trade Data (historical_data.csv)
Contains detailed records of individual trades, including:
-Account identifier
-Coin traded
-Execution price
-Trade size (tokens & USD)
-Direction (Long / Short)
-Timestamp (IST)
-Closed PnL
-Fees and trade metadata

2️⃣ Fear & Greed Index (fear_greed_index.csv)
-Daily market sentiment index with:
-Date
-Fear & Greed value
-Sentiment classification (Fear / Neutral / Greed)

🛠️ Methodology
Step 1: Data Exploration & Validation
-Inspected column names, data types, and missing values
-Verified that no assumed or synthetic data was used
Step 2: Timestamp Normalization
-Converted trade timestamps from DD-MM-YYYY (IST) format
-Standardized both datasets to a common daily date level
Step 3: Data Integration
-Merged trade data with daily Fear & Greed sentiment using date alignment
Step 4: Feature Engineering
-Created win/loss indicator based on Closed PnL
-Aggregated metrics at sentiment and trader levels
Step 5: Analysis & Insights
-Compared performance metrics across sentiment regimes
-Analyzed trader behavior, win rate, and profitability
-Identified directional bias during Fear vs Greed markets

📈 Key Insights
-Trader performance varies significantly across market sentiment regimes
-Certain sentiment conditions show higher average PnL and win rates
-Directional bias (Long vs Short) changes noticeably between Fear and Greed periods
-Market psychology plays a measurable role in trading outcomes
