# Cellular-V2X-Research

## 📖 Overview
This repository contains the Python-based simulation framework developed as my B.Sc. thesis project in Electrical and Electronic Engineering (EEE). It evaluates and optimizes Cellular V2X (C-V2X) link performance in dense urban deployment scenarios, specifically focusing on vehicle-to-infrastructure (V2I) and vehicle-to-vehicle (V2V) communications.

## ✨ Key Features
* **Spatial Deployment Model:** Simulates random placement of Base Stations (BS), V2I, and V2V nodes in a Manhattan Grid layout ($500\text{ m} \times 500\text{ m}$ to $800\text{ m} \times 800\text{ m}$).
* **Wireless Propagation & Path Loss:** Integrates both Line-of-Sight (LOS) and Non-Line-of-Sight (NLOS) attenuation models based on distance.
* **Interference Management:** Computes real-time Signal-to-Interference-plus-Noise Ratio (SINR) and interference matrices across orthogonal Resource Blocks (RBs).
* **Optimization Algorithms:** 
  * Baseline Fixed Resource Allocation & Uniform Power Control.
  * Dynamic Resource Allocation with Adaptive Power Control to mitigate V2V co-channel interference.

## 📊 Results & Performance
The dynamic resource allocation algorithm significantly outperforms the fixed baseline by intelligently distributing channels and scaling transmit power:

* **V2I Link Capacity:** Resolves severe throughput bottlenecks caused by co-channel interference, improving worst-case channel capacity from $\approx 0.41\text{ Mbps}$ to $\approx 4.30\text{ Mbps}$.
* **V2V Link Capacity:** Achieves higher minimum throughput across channels by dynamically adjusting transmit power (ranging from $10\text{ dBm}$ to $23\text{ dBm}$) and distributing RBs effectively.

## 🛠️ Prerequisites
Ensure you have Python 3.x installed along with the following libraries:
* `numpy`
* `pandas`
* `matplotlib`
* `scipy`
