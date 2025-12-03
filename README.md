**📊 COVID-19 Dashboard**

This project is an **interactive COVID-19 dashboard** built using **Python, Dash, and Plotly**.  
It visualizes important pandemic-related data using bar charts, line charts, and pie charts.  
Users can interact with dropdown menus to explore confirmed, recovered, deceased, and other commodity-based statistics.

**🚀 Project Features**

**✅ 1. Total Case Overview**

Displays four key metrics:

- **Total Cases**
- **Active Cases**
- **Recovered Cases**
- **Total Deaths**

Each metric is shown in a colored Bootstrap card.

**✅ 2. Interactive Graphs**

The dashboard contains multiple interactive visualizations:

**a) Line Chart**

Shows commodity-wise COVID data (Mask, Sanitizer, Oxygen, etc.)

**b) Pie Chart**

Shows distribution of:

- Red Zone
- Blue Zone
- Green Zone
- Orange Zone

**c) Bar Chart**

Displays COVID case statistics based on:

- Hospitalized
- Recovered
- Deceased
- All State Counts

All graphs update dynamically using Dash callbacks.

**📁 Project Structure**

COVID-Dashboard/

├── app.py

├── state_wise_daily.csv

├── README.md

- **app.py** → Main dashboard application
- **state_wise_daily.csv** → Dataset used for visualizations
- **README.md** → Documentation file (this file)

**🛠️ Technologies Used**

| **Library**   | **Purpose** |
| **Dash**      | Build interactive web dashboard |
| **Plotly**    | Create graphs and visualizations |
| **Pandas**    | Data loading & manipulation |
| **NumPy**     | Numerical operations |
| **Bootstrap** | Styling the dashboard |

**📥 Installation & Setup**

**1\. Clone the Project**

git clone <https://github.com/shyamsundar851/covid-dashboard.git>

cd covid-dashboard

**2\. Install Requirements**

pip install dash plotly pandas numpy

**3\. Add the Dataset**

Make sure the file **state_wise_daily.csv** is in the same folder as app.py.

**4\. Run the Application**

python app.py

**5\. Open in Browser**

Visit the link displayed in terminal, usually:

<http://127.0.0.1:8050/>

**🔧 How It Works**

The app uses **Dash callbacks** to update charts:

@app.callback(Output('bar','figure'), \[Input('picker','value')\])

Each dropdown value triggers a data update, and the graph refreshes automatically.

**📌 Future Improvements**

- Add real-time API data
- Deploy on Heroku or Render
- Add more visualizations
- Improve UI theme

**💡 Author**

**Shyam Sundar Pareek**
