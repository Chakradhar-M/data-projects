# **AirPure Market Fit Analysis – Primary, Secondary & Strategic Insights**


**Tool Used:** Google Colab (Python)


This document presents data-driven answers to the Primary, Secondary, and Strategic questions outlined in the *AirPure Market Research Challenge*. The insights are derived from AQI, health, population, and vehicle datasets covering 2022 to 2025, analyzed using Python in Google Colab. Each question is addressed with concise interpretations supported by visualizations and evidence.


## **Primary Analysis**

### **Q1. Which 5 areas recorded the highest and lowest average AQI between Dec 2024 and May 2025?**

**Insight:**
The most polluted areas during this period were concentrated in **northern and eastern India**, led by **Byrnihat (Assam)** and **Delhi**. Southern cities like **Tirunelveli (Tamil Nadu)** and **Madikeri (Karnataka)** reported the cleanest air.


**Top 5 Areas with Highest Avg AQI**

| State   | Area        | Avg AQI |
| ------- | ----------- | ------- |
| Assam   | Byrnihat    | 284.19  |
| Delhi   | Delhi       | 238.92  |
| Bihar   | Hajipur     | 233.67  |
| Haryana | Bahadurgarh | 226.44  |
| Haryana | Gurugram    | 204.14  |


**Bottom 5 Areas with Lowest Avg AQI**

| State      | Area           | Avg AQI |
| ---------- | -------------- | ------- |
| Tamil Nadu | Tirunelveli    | 33.31   |
| Tamil Nadu | Palkalaiperur  | 42.79   |
| Karnataka  | Madikeri       | 42.95   |
| Karnataka  | Vijayapura     | 44.33   |
| Karnataka  | Chamarajanagar | 44.81   |

---


### **Q2. What are the top 2 and bottom 2 dominant pollutants in each southern Indian state (2022 onwards)?**

**Insight:** Across Southern India, **PM10**, **PM2.5** is consistently the most frequent pollutant. Rare combinations involving gases like **NO2**, **CO**, and **NH3** appear the least. This helps tailor filter design to local pollutant profiles.


> *Note: Some pollutants appear as combinations (e.g., PM2.5,PM10). These represent co-dominant pollutants observed at the same location and time. They are retained to reflect real-world AQI reporting patterns.*


#### **Andhra Pradesh**

| Type   | Prominent Pollutant | Count |
| ------ | ------------------- | ----- |
| Top    | PM10                | 3182  |
|        | PM2.5               | 1757  |
| Bottom | PM10,NO2,O3         | 1     |
|        | PM10,NO2,PM2.5,O3   | 1     |



#### **Karnataka**

| Type   | Prominent Pollutant | Count |
| ------ | ------------------- | ----- |
| Top    | PM10                | 13404 |
|        | CO                  | 2913  |
| Bottom | NO2,O3              | 1     |
|        | NO2,SO2,CO          | 1     |



#### **Kerala**

| Type   | Prominent Pollutant | Count |
| ------ | ------------------- | ----- |
| Top    | PM10                | 3167  |
|        | PM2.5               | 1123  |
| Bottom | CO,O3               | 6     |
|        | SO2                 | 7     |



#### **Puducherry**

| Type   | Prominent Pollutant | Count |
| ------ | ------------------- | ----- |
| Top    | PM10                | 413   |
|        | O3                  | 303   |
| Bottom | CO                  | 148   |
|        | PM2.5               | 206   |



#### **Tamil Nadu**

| Type   | Prominent Pollutant | Count |
| ------ | ------------------- | ----- |
| Top    | PM10                | 6253  |
|        | PM2.5               | 2268  |
| Bottom | PM10,NH3,CO         | 1     |
|        | PM10,NO2,PM2.5,O3   | 1     |



#### **Telangana**

| Type   | Prominent Pollutant | Count |
| ------ | ------------------- | ----- |
| Top    | PM2.5,PM10          | 343   |
|        | PM10                | 315   |
| Bottom | CO,O3               | 1     |
|        | NO2                 | 1     |

---

### **Remaining Primary Questions**

3. Is there a noticeable difference in AQI levels between weekdays and weekends in major metro cities?
4. Which months consistently record the poorest air quality across the top 10 states (by area count)?
5. How many days in Bengaluru fell under each AQI category from March to May 2025?
6. What are the top two most reported illnesses in each state over the last 3 years, and their average AQI?
7. Do the top 5 states with highest EV adoption show significantly better AQI than low-EV states?

---

---
## **Secondary Analysis**

1. Which age group is most affected by pollution-related health issues, and how does this vary by city?
2. Who are the key players in the Indian air purifier market, and what features set them apart?
3. Is there a relationship between a city’s population size and its average AQI in 2024?
4. How well do Indian citizens understand AQI and its health implications?
5. Which government policies in the past 5 years have most effectively improved air quality, and where?

---

## **Strategic (Critical) Questions**

1. Which Tier 1 and Tier 2 cities show signs of irreversible AQI deterioration?
2. How do AQI spikes correlate with pediatric asthma admissions across regions?
3. Do pollution emergencies drive increased air purifier interest or purchase behavior?
4. What key features are missing in current air purifier products?

---

Let me know if you want this copy as a `.md`, `.docx`, or Google Doc.

