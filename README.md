# **Detecting Fake Vehicles Using V2X Communication**

## **Overview**
This project focuses on detecting **fake vehicles** in a V2X (Vehicle-to-Everything) communication network using **machine learning**. Fake vehicles result from **sensor spoofing**, where attackers inject false data into a vehicle's communication system. This can cause significant issues, such as traffic accidents, manipulation of traffic patterns, and potential security breaches in autonomous systems.

## **The Problem: Sensor Spoofing**
Sensor spoofing involves manipulating the data transmitted by a vehicle, making it appear as though the vehicle is behaving in a normal, expected way when it is not. This can affect several aspects of vehicle behavior:
- **GPS Spoofing**: Fake location data, causing the vehicle to appear in different locations.
- **Speed and Acceleration**: Erratic or impossible speed and acceleration patterns.
- **Communication Interference**: Fake vehicles can overload the V2X network with false messages or fail to communicate properly with nearby vehicles.

These fake vehicles pose a danger to real vehicles on the road and disrupt the V2X communication network.

## **Solution: Machine Learning Detection**
This repository offers a solution using a **Random Forest Classifier** to detect fake vehicles. By analyzing key features such as:
- **V2X Communication Patterns**
- **GPS Consistency**
- **Signal Strength**
- **Behavioral Consistency**

The model can classify vehicles as either **real** or **fake** based on these patterns.

## **How It Works**
1. **Data Collection**: The system gathers data from both real and fake vehicles in a V2X network.
2. **Feature Engineering**: Key behavioral features are extracted from the dataset (e.g., communication success rate, GPS data).
3. **Model Training**: The Random Forest model is trained on labeled data to learn the differences between real and fake vehicles.
4. **Prediction**: The model evaluates new data to detect whether a vehicle is fake.

## **Conclusion**
This project provides a machine learning-based approach to detect fake vehicles in V2X communication networks, improving road safety and communication integrity by preventing sensor spoofing attacks.
