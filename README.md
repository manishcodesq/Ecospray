# Intelligent Pesticide Sprinkling System 🌱

An **AI + IoT enabled smart pesticide spraying solution** designed for sustainable farming.  
This project uses **ESP32-CAM**, IoT sensors, and a **Machine Learning model** to detect plant diseases, classify infection severity, and intelligently control pesticide spraying. A **React + Tailwind farmer dashboard** provides real-time insights, reports, and cost savings.

---

## 🚀 Features
- 🌾 **AI-Powered Detection** – Classifies plant health (Healthy / Mild / Severe infection) using a CNN model.  
- 💧 **Smart Spraying** – Solenoid valves adjust spray dosage based on infection severity.  
- 📊 **Farmer Dashboard** – React + Tailwind dashboard with heatmaps, pesticide savings %, and compliance reports.  
- 🌍 **Low-Cost Retrofit** – Built on **ESP32-CAM** and sensors for smallholder farmer affordability.  
- 🔄 **Closed-Loop Verification** – Re-scan after spraying to confirm effectiveness.  
- ☁️ **Hybrid Edge + Cloud** – TinyML inference on ESP32 + cloud retraining via Express backend.  

---

## 🛠️ Tech Stack

**Hardware Components**
- ESP32-CAM (image capture + TinyML inference)  
- Solenoid valve + Nozzle (controlled spraying)  
- Soil moisture, humidity, and temperature sensors  

**Software Components**
- **Frontend**: React + Tailwind (farmer dashboard)  
- **Backend**: Flask (APIs, device communication, cloud retraining)  
- **Database**: MongoDB(crop data, logs, farmer history)  
- **ML Model**: CNN (disease detection + severity scoring), quantized for TinyML  

---

## 📐 System Architecture
1. ESP32-CAM captures plant images and runs local ML inference.  
2. IoT sensors provide environmental context (soil, humidity, temp).  
3. ESP32 sends inference + sensor data to Express backend.  
4. Backend logs data, updates farmer dashboard, and triggers cloud retraining.  
5. ESP32 actuates solenoid nozzle to spray dosage based on infection severity.  
6. Farmer dashboard displays heatmaps, pesticide savings, and downloadable reports.  

---

## 📊 Research Gaps Addressed
- ❌ High-cost robotic/drones → ✅ **Low-cost ESP32 retrofit**  
- ❌ Binary spraying only → ✅ **Severity-based intelligent dosing**  
- ❌ RGB-only detection → ✅ **Multi-modal IoT data fusion**  
- ❌ No farmer UI → ✅ **Farmer dashboard with reports & insights**  
- ❌ No verification → ✅ **Closed-loop feedback mechanism**  

---

## 📦 Project Structure
