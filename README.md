# 🚦 Traffic Flow Prediction Using GAN (Project)

This project presents a deep learning approach to predict traffic conditions at neighboring intersections using a **Generative Adversarial Network (GAN)**. 
The simulation environment is built in **SUMO (Simulation of Urban MObility)**, structured as a 4x4 urban grid, and the GAN model is trained on simulation-generated traffic data.

## 📚 project Objective

The aim of this project is to improve decentralized traffic signal control by **predicting future traffic flow at adjacent intersections**. 
This predictive approach reduces the dependency on real-time communication between intersections, which is often costly and bandwidth-limited.

## 🧠 What the GAN Does

- **Input**: Real-time traffic data from a local intersection, including:
  - Vehicle count per lane
  - Average speed per lane
  - Current signal state (green/red)
  - Time of day (morning/evening)

- **Output**: Predicted vehicle count for **neighboring intersections** in the next few seconds.

- **Goal**: To enable each intersection to anticipate traffic inflow from its neighbors and make proactive decisions (e.g., adjust green/red timing) without needing direct communication.

The GAN consists of:
- A **Generator** that learns to predict plausible future traffic conditions based on current input.
- A **Discriminator** that tries to distinguish real traffic data from generated predictions, forcing the Generator to improve.

---

## 🛠️ Technologies & Tools

- 🧠 **Machine Learning**: PyTorch
- 🚗 **Traffic Simulation**: SUMO
- 📊 **Data Processing**: Pandas, NumPy
- 📈 **Visualization**: Matplotlib, Seaborn
- 📂 **Data Format**: CSV (tabular lane-wise traffic data)
- 🧪 **Network Setup**: 4x4 grid with `.net.xml`, `.rou.xml`, `.trips.xml`, `.sumocfg` files

---
