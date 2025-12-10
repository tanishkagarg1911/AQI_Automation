# 🌿 Air Quality Monitoring & Automation Pipeline (Indian Cities)

## 📄 Project Description
This project automatically fetches real-time air quality data (AQI) for **Indian** using the [AQICN API](https://aqicn.org/data-platform/token-confirm/eeb10b1b-54fd-4938-9d7a-16296780ea78), stores it in a CSV file, analyzes trends, and visualizes **PM2.5** levels with rolling averages.  

It provides insights on daily air quality and can be scheduled to run **hourly** for continuous monitoring.

---

## 🛠 Technologies Used
- **Python 3** – main programming language  
- **Requests** – fetch data from WAQI API  
- **Pandas** – data cleaning, manipulation, rolling averages  
- **Matplotlib** – plotting PM2.5 trends  
- **Schedule** – automated hourly updates  
- **CSV** – persistent data storage  

**Optional advanced:** Telegram / Email Alerts, Streamlit / Plotly Dash dashboards, Deployment on PythonAnywhere or cloud VM  

---

## ✨ Features
- Automated hourly data collection from AQI API  
- CSV storage with duplicate removal and data cleaning  
- Rolling averages for PM2.5 trend analysis  
- Graphical visualization of PM2.5 trends over time  
- Day-wise insights: best/worst air quality  
- Scheduler-enabled for continuous operation  

---
