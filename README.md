<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Air Quality Monitoring & Automation Pipeline</title>
</head>
<body>
    <h1 style="text-align:center;">🌿 Air Quality Monitoring & Automation Pipeline (Delhi) 🌿</h1>

    <h2>📄 Project Description</h2>
    <p>
        This project automatically fetches real-time air quality data (AQI) for Delhi using the 
        <a href="https://aqicn.org/data-platform/token/" target="_blank">World Air Quality Index (WAQI) API</a>, 
        stores it in a CSV file, analyzes trends, and visualizes PM2.5 levels with rolling averages. 
        It provides insights on daily air quality and can be scheduled to run hourly for continuous monitoring.
    </p>
    
    <h2>🛠 Technologies Used</h2>
    <ul>
        <li>Python 3 – main programming language</li>
        <li>Requests – fetch data from WAQI API</li>
        <li>Pandas – data cleaning, manipulation, rolling averages</li>
        <li>Matplotlib – plotting PM2.5 trends</li>
        <li>Schedule – automated hourly updates</li>
        <li>CSV – persistent data storage</li>
    </ul>
    <p><strong>Optional advanced:</strong> Telegram / Email Alerts, Streamlit / Plotly Dash dashboards, Deployment on PythonAnywhere or cloud VM</p>
    
    <h2>✨ Features</h2>
    <ul>
        <li>Automated hourly data collection from AQI API</li>
        <li>CSV storage with duplicate removal and data cleaning</li>
        <li>Rolling averages for PM2.5 trend analysis</li>
        <li>Graphical visualization of PM2.5 trends over time</li>
        <li>Day-wise insights: best/worst air quality</li>
        <li>Scheduler-enabled for continuous operation</li>
    </ul>
    
    <h2>⚙️ Setup & Installation</h2>
    <ol>
        <li>Clone the repository:
            <pre>git clone &lt;your-repo-link&gt;</pre>
        </li>
        <li>Install dependencies:
            <pre>pip install requests pandas matplotlib schedule</pre>
        </li>
        <li>Get WAQI API key from <a href="https://aqicn.org/data-platform/token/" target="_blank">WAQI Data Platform</a></li>
        <li>Set API key in <code>demo.py</code>:
            <pre>API_KEY = "&lt;YOUR_API_KEY&gt;"</pre>
        </li>
        <li>Run the project:
            <pre>python demo.py</pre>
        </li>
    </ol>
    
    <h2>📌 Usage</h2>
    <ul>
        <li>Fetches real-time AQI data for Delhi.</li>
        <li>Saves readings in <code>air_quality_data.csv</code>.</li>
        <li>Cleans data, computes PM2.5 rolling trends.</li>
        <li>Plots trends and prints insights to console.</li>
        <li>Scheduler runs the pipeline every hour automatically.</li>
    </ul>
    <p><strong>Optional:</strong> Change <code>CITY</code> variable to monitor other cities, enable alerts for high AQI.</p>

    <h2>📊 Sample Output</h2>
    <p><strong>Console Insights:</strong></p>
    <pre>
Dominant pollutant today (PM2.5 avg): 161
Day with worst AQI: 2025-12-10
Day with best AQI: 2025-12-09
    </pre>
    <p><strong>CSV Sample:</strong></p>
    <pre>
city,aqi,pm25,pm10,o3,no2,timestamp
delhi,161,161,124,48.8,19.9,2025-12-10 13:00:00
delhi,159,159,120,50.0,20.1,2025-12-10 14:00:00
    </pre>

    <h2>🚀 Future Improvements</h2>
    <ul>
        <li>Add real-time alerts via Telegram or email for high AQI levels.</li>
        <li>Host live dashboards using Streamlit or Plotly Dash.</li>
        <li>Store historical data in a database for long-term trend analysis.</li>
        <li>Extend monitoring to multiple cities simultaneously.</li>
    </ul>

    <h2>👥 Credits</h2>
    <ul>
        <li>Data Source: World Air Quality Index Project (WAQI)</li>
        <li>Developed by: &lt;Your Name&gt;</li>
    </ul>
</body>
</html>
