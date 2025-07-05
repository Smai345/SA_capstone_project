# 🚗 Dynamic Parking Pricing Engine

## 📌 Project Overview
This project implements a real-time, data-driven dynamic pricing system for urban parking lots. It adjusts parking fees based on occupancy, traffic conditions, and other demand signals to maximize revenue while maintaining optimal utilization of parking spaces. The project compares two models:
- **Model 1:** Baseline Linear Pricing
- **Model 2:** Demand-Based Pricing

---

## 💻 Tech Stack
- **Python 3**: Core implementation language
- **Pandas & Numpy**: Data preprocessing and manipulation
- **Pathway**: Real-time data stream processing, windowing, and aggregation
- **Bokeh**: Interactive, real-time plotting of pricing data
- **Google Colab**: Development and experimentation environment
- **Git/GitHub**: Version control and project hosting

---

## 🏗️ Architecture Diagram
```mermaid
flowchart TD
    A[CSV Data (parking_stream.csv)] --> B[Pathway Data Stream]
    B --> C1[Model 1: Baseline Linear Pricing]
    B --> C2[Model 2: Demand-Based Pricing]
    C1 --> D1[Bokeh Plot: Baseline Prices]
    C2 --> D2[Bokeh Plot: Demand Prices]
