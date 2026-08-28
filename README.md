# 🚲 Bike Sharing Dashboard

An interactive dashboard for analyzing and visualizing **Bike Sharing Dataset** using Python and Streamlit. This project explores bike rental patterns based on weather conditions, working days, weekdays, and seasons.

The dashboard allows users to filter the analysis based on a selected date range and explore rental trends through statistical summaries and interactive visualizations.

---

## 📌 Project Overview

Bike-sharing systems provide an alternative mode of transportation in urban areas. Understanding rental patterns can help identify factors that influence bike usage and provide insights into user behavior.

This project analyzes bike-sharing rental data to answer several questions:

* How does **weather condition** affect the number of bike rentals?
* How do bike rentals differ between **working days and non-working days**?
* Which **day of the week** has the highest average bike rentals?
* How does the **season** affect casual and registered bike users?
* What patterns can be observed from bike rental activity over different periods?

The results are presented through a web-based dashboard built with **Streamlit**.

---

## 🎯 Business Questions

This dashboard focuses on the following analytical questions:

### 1. Weather Impact

How does the weather condition relate to the number of bike rentals?

### 2. Working Day Impact

Is there a difference in bike rental activity between working days and non-working days?

### 3. Weekday Pattern

Which day of the week has the highest and lowest average number of bike rentals?

### 4. Seasonal Pattern

How do casual and registered users differ across seasons?

---

## 📊 Dataset

This project uses the **Bike Sharing Dataset**, which contains information about bike rental counts along with environmental and seasonal variables.

The dataset is divided into two files:

* `day.csv` — daily bike rental data
* `hour.csv` — hourly bike rental data

### Main Variables

| Variable     | Description                      |
| ------------ | -------------------------------- |
| `dteday`     | Date                             |
| `season`     | Season category                  |
| `yr`         | Year                             |
| `mnth`       | Month                            |
| `holiday`    | Whether the day is a holiday     |
| `weekday`    | Day of the week                  |
| `workingday` | Whether the day is a working day |
| `weathersit` | Weather condition                |
| `temp`       | Normalized temperature           |
| `atemp`      | Normalized feeling temperature   |
| `hum`        | Normalized humidity              |
| `windspeed`  | Normalized wind speed            |
| `casual`     | Number of casual users           |
| `registered` | Number of registered users       |
| `cnt`        | Total number of bike rentals     |

---

## 🔎 Data Analysis

### Weather Condition vs Bike Rentals

The dashboard groups bike rental data based on `weathersit` and calculates:

* Mean rental count
* Total rental count
* Maximum rental count
* Minimum rental count

A boxplot is also used to visualize the distribution of bike rentals under different weather conditions.

---

### Working Day vs Non-Working Day

Bike rental activity is compared between:

* Working days
* Non-working days

The dashboard calculates the mean, total, maximum, and minimum rental counts for each category.

A bar chart is used to visualize the comparison.

---

### Bike Rentals by Weekday

The dashboard analyzes the average number of rentals for each day of the week.

The analysis provides:

* Mean rental count
* Total rental count
* Maximum rental count
* Minimum rental count

A line chart is used to visualize the average rental activity across weekdays.

---

### Seasonal Analysis

Bike rental activity is analyzed across different seasons.

The dashboard compares:

* Total casual users by season
* Total registered users by season
* Average casual users by season
* Average registered users by season

This helps identify differences in usage patterns between casual and registered users across seasons.

---

## 📈 Dashboard Features

The dashboard provides:

* 📅 **Date range filtering**
* 🌦️ **Weather condition analysis**
* 💼 **Working day analysis**
* 📆 **Weekday rental analysis**
* 🌱 **Seasonal rental analysis**
* 📊 **Statistical summary tables**
* 📉 **Data visualizations**
* 🖥️ **Interactive Streamlit interface**

---

## 🛠️ Tech Stack

### Programming Language

* Python

### Data Processing

* Pandas
* NumPy

### Data Visualization

* Matplotlib
* Seaborn

### Dashboard

* Streamlit

### Development Environment

* Jupyter Notebook / Google Colab
* Visual Studio Code

---

## 📁 Project Structure

```text
bike-sharing-dashboard/
│
├── data/
│   ├── day.csv
│   └── hour.csv
│
├── dashboard/
│   ├── dashboard.py
│   └── requirements.txt
│
├── README.md
└── .gitignore
```

---

## ⚙️ Installation & Setup

### 1. Clone Repository

```bash
git clone https://github.com/USERNAME/bike-sharing-dashboard.git
```

Navigate to the project directory:

```bash
cd bike-sharing-dashboard
```

Then enter the dashboard directory:

```bash
cd dashboard
```

---

### 2. Create Virtual Environment

Create a Python virtual environment:

```bash
python -m venv env
```

Activate the virtual environment.

**Windows:**

```bash
env\Scripts\activate
```

**macOS/Linux:**

```bash
source env/bin/activate
```

---

### 3. Install Dependencies

Install the required Python packages:

```bash
pip install -r requirements.txt
```

---

## ▶️ Run the Dashboard

From the `dashboard` directory, run:

```bash
streamlit run dashboard.py
```

After the application starts, open the URL displayed in the terminal.

Usually:

```text
http://localhost:8501
```

---

## 📦 Requirements

The main libraries used in this project include:

```text
numpy
pandas
matplotlib
seaborn
streamlit
```

The complete package versions are available in:

```text
dashboard/requirements.txt
```

---

## 📝 Updating Requirements

If additional Python packages are installed or the environment is updated, the `requirements.txt` file can be regenerated using:

```bash
pip freeze > requirements.txt
```

---

## 💡 Key Insights

Based on the analysis presented in the dashboard, several patterns can be explored:

* Bike rental activity varies across different weather conditions.
* Rental patterns differ between working days and non-working days.
* Bike usage is not evenly distributed across all days of the week.
* Seasonal conditions influence both casual and registered user activity.
* Registered users generally represent a substantial portion of total bike rentals.

> **Note:** The dashboard allows users to explore these patterns dynamically based on the selected date range.

---

## 🚀 Future Improvements

Potential improvements for this project include:

* Adding monthly and yearly rental trend analysis.
* Adding temperature, humidity, and wind speed analysis.
* Adding interactive Plotly visualizations.
* Adding separate analysis for casual and registered users.
* Adding KPI cards for total rentals, average rentals, and user composition.
* Adding predictive modeling to forecast future bike rental demand.
* Improving dashboard layout and visual design.

---

## 👩‍💻 Author

**Syifa Arifah Nurbayani**

Informatics Engineering Graduate | Data Science & Machine Learning Enthusiast

### Skills

* Python
* Data Analysis
* Machine Learning
* Data Visualization
* Natural Language Processing
* Streamlit
* Pandas
* NumPy
* Matplotlib
* Seaborn

---

## 📄 License

This project is intended for educational and portfolio purposes.
