Modeling Safe Detection Distance for Road Hazard Prevention
===========================================================

### **Project Overview**

This project presents a data-driven policy framework for mitigating road accidents under low-visibility conditions (fog, mist, and nighttime). By combining kinematic physics modeling with empirical accident data from the **Ministry of Road Transport and Highways (MoRTH)**, the study identifies critical "unsafe regions" where required stopping distance exceeds human visual range.

### **Core Problem**

In India, particularly in North Indian highway corridors like **NH-44 and the Yamuna Expressway**, dense winter fog frequently leads to multi-vehicle collisions. Current static speed limits often fail to account for the non-linear relationship between speed, reaction time, and friction, creating a structural mismatch between visibility and vehicle dynamics.

### **Key Findings**

*   **Non-Linear Risk**: Stopping distance rises non-linearly with speed; beyond certain thresholds, safe stopping becomes physically impossible.
    
*   **Dense Fog (~20m visibility)**: Safe stopping is limited to $\\approx40\\text{ km/h}$; exceeding this speed makes collision avoidance physically infeasible.
    
*   **Moderate Fog (~40m visibility)**: The safe threshold is $\\approx60\\text{ km/h}$.
    
*   **Low-Visibility Night (~70m visibility)**: Safe thresholds drop to $\\approx90\\text{ km/h}$, yet highway speeds often exceed this, contributing to a high share of night-time fatalities.
    

### **Proposed Solution: Dynamic Digital Infrastructure**

The study proposes a transition to **Dynamic Speed Regulation** through:

1.  **Edge-Based Processing**: Utilizing lightweight backend frameworks (e.g., **FastAPI**) to ingest real-time visibility sensor data and compute safe speed thresholds locally.
    
2.  **Variable Message Signs (VMS)**: Deploying roadside digital signage to display visibility-based speed limits in real-time.
    
3.  **Predictive Policy**: Aligning speed limits with physical safety constraints derived from localized environmental monitoring.
    

### **Technical Implementation**

The repository includes:

*   road\_safety\_model.py: A Python-based simulation evaluating stopping distances across multiple speeds (20–100 km/h), reaction times (0.8–1.5s), and road conditions (Dry/Wet).
    
*   Policy\_Brief.pdf: The full comprehensive report optimized for policy evaluation.
    

### **References**

*   **Ministry of Road Transport and Highways (MoRTH)**: Road Accidents in India 2022.
    
*   **AASHTO**: Policy on Geometric Design of Highways and Streets.
    
*   **PIARC**: Road Safety and Human Factors Guidelines.
