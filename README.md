 #🚕 NYC Taxi Big Data Visualization

## 📌 Overview

This project demonstrates a scalable end-to-end pipeline for processing and visualizing large-scale transportation data using modern Python big data tools. It leverages the NYC Taxi Trip dataset (50M+ records) to showcase how distributed computing and optimized data formats enable efficient analysis and interactive exploration.

The system integrates data ingestion, distributed processing, optimized storage, and high-performance visualization into a unified workflow.

---

 ##🎯 Key Objectives

* Efficiently process large-scale datasets using distributed computing
* Optimize storage using columnar data formats
* Visualize millions of records without performance issues
* Provide an interactive dashboard for data exploration

---

## 🧰 Tech Stack

| Tool       | Role                        |
| ---------- | --------------------------- |
| PySpark    | Distributed data processing |
| Dask       | Parallel data loading       |
| Datashader | Large-scale visualization   |
| Streamlit  | Interactive web dashboard   |
| Parquet    | Efficient columnar storage  |

---

## 🏗️ Architecture

```
Raw Data (NYC Taxi Dataset)
        ↓
PySpark (Cleaning & Processing)
        ↓
Parquet (Optimized Storage)
        ↓
Dask (Lazy Loading)
        ↓
Datashader (Visualization Engine)
        ↓
Streamlit (Interactive Dashboard)
```

---

## 📂 Project Structure

```
nyc-taxi-bigdata-visualization/
│
├── data/
│   ├── raw/            # Original dataset
│   └── processed/      # Cleaned & transformed data
│
├── src/
│   ├── data/           # Data handling utilities
│   ├── processing/     # PySpark processing logic
│   ├── visualization/  # Datashader logic
│   └── app/            # Streamlit dashboard
│
├── scripts/            # Execution scripts
├── outputs/            # Generated visualizations
├── docs/               # Documentation
├── requirements.txt
└── README.md
```

---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/nyc-taxi-bigdata-visualization.git
cd nyc-taxi-bigdata-visualization
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 📥 Dataset

The dataset is provided by the NYC Taxi and Limousine Commission.

Due to its large size, it is not included in this repository.

### Download Dataset

```bash
python scripts/download_data.py
```

---

## ⚡ Usage

### 1. Run Data Processing (PySpark)

```bash
python scripts/run_spark.py
```

### 2. Generate Visualizations (Datashader)

```bash
python scripts/run_datashader.py
```

### 3. Launch Dashboard (Streamlit)

```bash
streamlit run src/app/streamlit_app.py
```

---

## 📊 Features

* Handles datasets with 50M+ rows efficiently
* Distributed processing using PySpark
* Memory-efficient storage with Parquet
* Scalable visualization with Datashader
* Interactive dashboard with Streamlit

---

## 🖼️ Results

### Taxi Pickup Density Map

High-resolution density visualization of taxi pickups across NYC.

### Interactive Dashboard

User-friendly interface for exploring trip data dynamically.

---

## 📈 Key Insights

* PySpark significantly improves processing performance for large datasets
* Datashader prevents overplotting and ensures clarity at scale
* Streamlit enables rapid development of interactive dashboards
* The pipeline supports efficient big data exploration workflows

---

## ⚠️ Limitations

* No real-time data streaming support
* Tested primarily in a local environment
* Dataset must be downloaded separately

---

## 🚀 Future Improvements

* Deploy on cloud platforms (AWS, Azure, GCP)
* Integrate real-time streaming (Kafka, Spark Streaming)
* Add machine learning models for predictions
* Enhance geospatial analysis and visualization

---

## 📚 Thesis Information

**Title:** Visualizing Large Datasets Using Big Data Libraries in Python
**Author:** Yonas Yadeta Chibsa
**Program:** MSc in Computer Science (Data Science)

---

## 📜 License

This project is licensed under the MIT License.

---

## 🙌 Acknowledgments

* NYC Taxi and Limousine Commission
* Open-source Python community
