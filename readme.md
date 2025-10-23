# Indian Airlines Ticket Price Analysis

<div align="center">
  
![Project Status: Complete](https://img.shields.io/badge/status-complete-green)
![Python](https://img.shields.io/badge/Python-3.9%2B-blue?logo=python)
![Tools](https://img.shields.io/badge/Tools-Pandas%20%7C%20Seaborn%20%7C%20Power%20BI-brightgreen)

</div>

An exploratory data analysis (EDA) of domestic flight prices in India. This project analyzes a dataset of over 300,000 flight bookings to uncover the key factors that influence ticket pricing.

## 📋 Table of Contents
- [Objective](#objective)
- [Analysis Highlights](#-analysis-highlights)
- [Power BI Dashboard](#-power-bi-dashboard)
- [Tools Used](#-tools-used)
- [Dataset](#-dataset)
- [Key Findings](#-key-findings)
- [How to Run This Project](#-how-to-run-this-project)

## Objective

Post-pandemic, and with rising fuel prices, the aviation market has seen significant price volatility. As an aviation enthusiast, I wanted to understand what truly drives ticket prices in India.

This project performs an in-depth exploratory data analysis (EDA) on flight ticket prices for India's top 6 metro areas to understand the key factors that influence pricing. The goal is to uncover patterns that can help travelers plan their bookings more efficiently.

## 📊 Analysis Highlights

The analysis, conducted in the `India Airlines Ticket Price Exploratory Analysis.ipynb` notebook, answers several key questions:

* ✈️ **Airline Market Share:** Which airlines (Vistara, Air India, etc.) operate the most flights in this dataset?
* 💰 **Price by Class:** How significant is the price difference between Economy and Business class?
* 📈 **Price vs. Booking Time:** How does the price change as the departure date (`days_left`) approaches?
* ⏳ **Price vs. Flight Duration:** What is the relationship between flight duration and ticket cost?
* 🗺️ **Route Analysis:** How do prices vary based on source (`source_city`) and destination (`destination_city`)?
* ⏰ **Time of Day:** Are there cheaper times to depart or arrive (Morning, Evening, Night)?
* 🛑 **Stops vs. Price:** How do non-stop, one-stop, and multi-stop flights compare in price?

## 🖥️ Power BI Dashboard

A comprehensive Power BI dashboard was created to visualize the findings interactively. It allows users to filter by airline, class, source, and destination to get a clear, dynamic view of the pricing landscape.

**[➡️ View the Dashboard (PDF Version)](./Indian%20Airline%20Ticket%20Prices%20Dashboard.pdf)**

## 🛠️ Tools Used

* **Python:** For the core analysis.
* **Pandas:** For data manipulation, cleaning, and analysis.
* **NumPy:** For numerical operations.
* **Matplotlib & Seaborn:** For static data visualization in the notebook.
* **Jupyter Notebook:** For iterative analysis and documentation.
* **Power BI:** For creating the interactive dashboard.

## 💾 Dataset

The dataset was sourced from **Kaggle** and was originally scraped from the "Ease My Trip" website.

* **Source:** [Kaggle Flight Price Prediction Dataset](https://www.kaggle.com/datasets/shubhambathwal/flight-price-prediction)
* **Content:** Contains 300,261 flight booking records.
* **Features:** Includes `airline`, `flight`, `source_city`, `destination_city`, `class`, `departure_time`, `arrival_time`, `duration`, `stops`, `days_left`, and `price`.
* **Date Range:** Data was collected for 50 days, from February 11 to March 31, 2022.

## 💡 Key Findings

1.  **Class is Key:** Business class (primarily offered by Vistara and Air India) is significantly more expensive than Economy. Vistara's business class is, on average, the most expensive.
2.  **Book in Advance:** Prices rise sharply within the last 20 days before departure. The "sweet spot" for booking appears to be 3-7 weeks in advance.
3.  **Cheapest Airline:** 'AirAsia' consistently offers the cheapest economy class tickets among the 6 airlines.
4.  **Stops Cost More:** Non-stop flights are generally the cheapest. Prices increase with one or more stops.
5.  **Timing Matters:** Flights departing late at night and arriving early in the morning tend to be cheaper.
6.  **Route Variations:** Delhi (due to high connectivity) appears to be one of the cheapest cities to fly from, while Hyderabad is one of the more expensive cities to fly *to*.

## 🚀 How to Run This Project

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git)
    cd YOUR_REPOSITORY_NAME
    ```
2.  **Create and activate a virtual environment (recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```
3.  **Install dependencies:**
    ```bash
    pip install pandas numpy matplotlib seaborn jupyterlab
    ```
4.  **Launch Jupyter Lab:**
    ```bash
    jupyter lab
    ```
5.  **Run the analysis:**
    Open `India Airlines Ticket Price Exploratory Analysis.ipynb` and run the cells.
6.  **View the dashboard:**
    Open `Indian Airline Ticket Prices Dashboard.pbix` with Power BI Desktop or view the included [PDF version](./Indian%20Airline%20Ticket%20Prices%20Dashboard.pdf).