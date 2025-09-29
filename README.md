# 🟢 Redundancy-Aware Sensor Fusion with Drift Detection (Toy Demo)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Kalidasan-2001/redundancy-aware-sensor-fusion/blob/main/notebooks/redundancy_sensor_fusion.ipynb)


---

## 📘 Overview

This project is a **toy example** demonstrating how **redundancy** and **sensor fusion** improve reliability in noisy measurement systems and enable **automatic drift detection**.

We simulate three sensors measuring the same hidden (latent) signal:
- All sensors have small random noise.  
- One sensor (**C**) develops a **drift fault** after time step 700.  
- Fusion and drift detection techniques identify and isolate the faulty sensor.

---

## ⚙️ Techniques Implemented

| Technique | Description | Purpose |
|------------|--------------|----------|
| **Mean Fusion** | Simple average of all sensor readings | Reduces random noise |
| **Weighted Fusion** | Gives more trust to stable sensors (lower variance) | Improves accuracy under noise |
| **Kalman Filter Fusion** | Predicts & updates estimates using uncertainty modeling | Dynamic, robust fusion |
| **Drift Detection** | Uses rolling residual z-scores | Flags sensors with persistent drift |
| **Adaptive Trust Visualization** | Plots changing sensor weights | Shows the system learning which sensor to trust |
| **Automatic Fault Report** | Summarizes detection results | Improves explainability |

---

## 📊 Key Results

✅ **Before Drift** — All sensors agree and fusion matches the true signal.  
⚠️ **After Drift** — Sensor C drifts upward; weighted & Kalman fusion resist the drift.  
🚨 **Drift Detection** — Residual analysis correctly flags Sensor C.  
📉 **Fusion Stability** — Rolling standard deviation shows fused signals are smoother.  
🎛️ **Adaptive Weights** — Trust for Sensor C drops after drift starts.  

---

## 🧩 Notebook Structure

1. **Simulation** – latent signal + noisy sensors  
2. **Visualization** – sensors & drift behavior  
3. **Fusion** – mean, weighted, and Kalman fusion  
4. **Stability Check** – rolling standard deviation  
5. **Drift Detection** – residual z-scores and fault flagging  
6. **Adaptive Trust** – sensor weight visualization  
7. **Automatic Reporting** – drift detection summary  
8. **Discussion** – analysis and takeaways  

---

