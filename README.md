# Enhancing Supply Chain Decision-Making and Strategic Planning using Machine Learning and Neural Networks

**By:** Anubhav Kumar Tiwary  
**PRN:** 2301208039  
**Semester 4:** Dissertation  
**Guided by:**  
- Prof. Vishnupant Potdar  
- Prof. Shubhangi P. Tidake

---

## 🚚 Project Overview

Timely deliveries can make or break your supply chain. In today’s fast world, a late shipment means disappointed customers and lost business. Old school methods just don’t cut it anymore. This project builds a smooth, data-driven pipeline using machine learning and neural networks to predict last-mile delivery times and help keep your supply chain running like a tuned engine.

We took a real-world Amazon delivery dataset, ran it through advanced preprocessing and engineered features that actually matter. We tested classic regression, bagging, forests, boosting, and deep learning. CatBoost grabbed the pole position with the best accuracy (R² of 0.8666) and performance. You’ll find no-nonsense model comparisons, clear insights, and actionable analytics to drive smarter supply chain decisions.

---

## 🔍 Problem Statement

Modern supply chains are a beast — unpredictable weather, traffic jams, human quirks. Missed ETAs hit customer loyalty and profits hard. Rule-based guesses are outdated.  
**We need** real-time, intelligent models that handle complexity and help decision-makers stay ahead of the curve.  
This research builds exactly that: a robust, scalable prediction engine using machine learning and neural networks, giving you the edge in delivery and planning.

---

## 📦 About the Dataset

**Source:** [Kaggle: Amazon Delivery Dataset](https://www.kaggle.com/datasets/sujalsuthar/amazon-delivery-dataset/data)  
- Covers over 43,600 real Amazon deliveries across Indian cities.
- Offers deep detail: order/agent info, weather, traffic, vehicle and area type, timestamps, and delivery performance.

**Key Columns:**
| Name           | Description                                 |
| -------------- | ------------------------------------------- |
| Order_ID       | Unique order number                         |
| Agent_Age      | Age of the delivery agent                   |
| Agent_Rating   | Performance score of the agent              |
| Store_Latitude | Store’s latitude                            |
| Store_Longitude| Store’s longitude                           |
| Drop_Latitude  | Customer’s latitude                         |
| Drop_Longitude | Customer’s longitude                        |
| Order_Date     | When the order was placed                   |
| Order_Time     | When the order was placed                   |
| Pickup_Time    | When the order was picked up                |
| Weather        | Delivery weather conditions                 |
| Traffic        | Delivery traffic conditions                 |
| Vehicle        | Type of vehicle used                        |
| Area           | Urban/Metropolitan/Semi-Urban/Other         |
| Delivery_Time  | Minutes taken to deliver                    |
| Category       | Product category                            |

---

## 🔧 Approach & Features

- **Preprocessing:**  
  Removed bad data, fixed types, handled outliers, and engineered new time & distance features.  
- **Feature Engineering:**  
  Converted timestamps to usable features, calculated true distance (Haversine), marked weekends, grouped age categories, and created dummies for categorical variables.
- **Exploratory Analysis:**  
  Pinpointed what really drives delays: agent age, ratings, traffic, weather, urban vs rural, and time of day.
- **Modeling:**  
  Trained and compared 9 models: Linear Regression, Decision Tree (Bagging), Random Forest, XGBoost, LightGBM (tuned with Optuna), CatBoost, SVR, Neural Network (MLP).  
- **Evaluation:**  
  Used 5-fold CV with R², MAE, MSE, and RMSE. CatBoost was the MVP (R²: 0.8666).

---

## 💡 Key Insights

- Younger, higher-rated agents delivered faster.
- Deliveries in 'Other' and Urban areas beat out Metropolitan and Semi-Urban.
- Evening and bad weather (cloudy, foggy) created max delays.
- Weekend vs. weekday didn’t make much difference.
- CatBoost’s predictions nailed most deliveries within a tight margin.

---

## 🚀 How to Use

- All code runs in Python (VS Code/Colab/Jupyter).
- Due to data and model size, raw files are not hosted here.  
- To try yourself:  
  1. Download [the dataset](https://www.kaggle.com/datasets/sujalsuthar/amazon-delivery-dataset/data)  
  2. Follow steps in this repo (see code, feature engineering, model training & evaluation)
  3. For more context, see the [publication](https://ijirt.org/Article?manuscript=182050)

---

## 📄 Publication

Want the detailed write-up and research validation? Check out the [IJIRT publication](https://ijirt.org/Article?manuscript=182050).

---

## 📬 Contact

For feedback, suggestions, or collaborations, reach out:  
[anubhavkumartiwary0109@gmail.com](mailto:anubhavkumartiwary0109@gmail.com)

---

*This repo connects data science with supply chain excellence—predict, optimize, and deliver.*
