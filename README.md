# 📊 ETL Pipeline to extract financial data

This repository contains project which was used to prepare case studies for my masters thesis: "Multifaceted comparative analysis of cloud platforms in CI/CD processes using performance-cost criteria" where I compared time, performance and CO2 emissions of different sizes of Virtual Machines available in Microsoft Azure, Amazon Web Services as well as Google Cloud Platform.

After running `docker compose up` command Python script will send a reqest to external REST API containing Stock Market Data, store it as Pandas dataframe and insert validated data to database. Data will contain open, close, low and high of particular day for the last 4 trading days.


## ✨ Technologies

- `Python`
- `PostgreSQL`
- `Docker`
- `GitHub Actions`

## 🚀 Features

- Extracting data from REST API
- Creating pandas dataframe where downloaded data are stored
- Validation of downloaded data
- Inserting data to PostgreSQL database
 
## 🚦 Running the Project

1. Clone the repository
2. Get your REST API key for Stock Market Data (https://www.alphavantage.co was used in the following example)
3. Set environment variables for `DB_PASS`, `POSTGRES_PASSWORD` and `API_KEY`
4. Run `docker compose up --abort-on-container-exit`
