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

**Insight:**

Across Southern India, **PM10**, **PM2.5** are consistently the most frequent pollutants. Rare combinations involving gases like **NO2**, **CO**, and **NH3** appear the least. This helps tailor filter design to local pollutant profiles.


> *Note: Some pollutants appear as combinations (e.g., PM2.5,PM10). These represent co-dominant pollutants observed at the same location and time. They are retained to reflect real-world AQI reporting patterns.*

#### Top 2 and Bottom 2 Prominent Pollutants in Southern Indian States (2022 Onwards)

| State         | Type    | Prominent Pollutant     | Count |
|---------------|---------|--------------------------|--------|
| Andhra Pradesh| Top     | PM10                     | 3182   |
|               |         | PM2.5                    | 1757   |
|               | Bottom  | PM10,NO2,O3              | 1      |
|               |         | PM10,NO2,PM2.5,O3        | 1      |
| Karnataka     | Top     | PM10                     | 13404  |
|               |         | CO                       | 2913   |
|               | Bottom  | NO2,O3                   | 1      |
|               |         | NO2,SO2,CO               | 1      |
| Kerala        | Top     | PM10                     | 3167   |
|               |         | PM2.5                    | 1123   |
|               | Bottom  | CO,O3                    | 6      |
|               |         | SO2                      | 7      |
| Puducherry    | Top     | PM10                     | 413    |
|               |         | O3                       | 303    |
|               | Bottom  | CO                       | 148    |
|               |         | PM2.5                    | 206    |
| Tamil Nadu    | Top     | PM10                     | 6253   |
|               |         | PM2.5                    | 2268   |
|               | Bottom  | PM10,NH3,CO              | 1      |
|               |         | PM10,NO2,PM2.5,O3        | 1      |
| Telangana     | Top     | PM2.5,PM10               | 343    |
|               |         | PM10                     | 315    |
|               | Bottom  | CO,O3                    | 1      |
|               |         | NO2                      | 1      |

---

### **Q3. Does AQI improve on weekends vs weekdays in Indian metro cities? (Consider data from last 1 year)**


**Insight:**

The difference in AQI between weekdays and weekends is **minor across most cities**. 

Notably:

* **Delhi** shows slight improvement on weekends (\~10 AQI drop).
* **Chennai** shows a small but clearer improvement.
* In cities like **Mumbai** and **Hyderabad**, AQI is slightly higher on weekends, possibly due to traffic from leisure and events.


**Average AQI by Day Type**

| City      | Weekday AQI | Weekend AQI |
| --------- | ----------- | ----------- |
| Delhi     | 208.70      | 198.92      |
| Ahmedabad | 114.72      | 116.04      |
| Pune      | 101.95      | 100.85      |
| Kolkata   | 91.73       | 91.26       |
| Mumbai    | 91.05       | 92.65       |
| Hyderabad | 77.92       | 79.01       |
| Bengaluru | 71.90       | 72.38       |
| Chennai   | 71.25       | 68.44       |


---

### Q4. Which months consistently show the worst air quality across Indian states
*(Consider top 10 states with high distinct areas)*  


#### Insight:
- **November** and **December** show the **worst air quality** across most states, particularly Bihar, Haryana, Odisha, and Uttar Pradesh.
- **January** also reflects high AQI, especially in northern states.
- **June to September** show significantly **cleaner air**, likely due to monsoon effects.

#### Possible Reasons:
- **Post-monsoon stubble burning** in Punjab, Haryana, and UP (Oct–Nov).
- **Winter smog** due to temperature inversion (Nov–Jan).
- **Diwali-related firecracker pollution** (usually in October/November).

#### Heatmap: Monthly Average AQI for Top 10 States  
![Monthly AQI Heatmap](https://github.com/Chakradhar-M/data-projects/blob/main/airpure_challenge/images/4Q_Heatmap_AQI_Month_City.png?raw=true)

---

### Q5. For the city of Bengaluru, how many days fell under each air quality category (e.g., Good, Moderate, Poor, etc.) between March and May 2025?

#### Insight:
Only two categories were observed during this period, indicating generally clean air in Bengaluru.

| Air Quality Category | Number of Days |
|----------------------|----------------|
| Satisfactory         | 48             |
| Moderate             | 13             |

> No days were recorded under **Good**, **Poor**, **Very Poor**, or **Severe** categories.

---


### **Q6) What are the top two most reported disease illnesses in each state over the past three years, and their corresponding average AQI?**

This analysis highlights the two most frequently reported diseases in each state (2022–2025), along with the associated average AQI. 


> **Note:**

> The most reported illnesses across states, such as **Acute Diarrheal Disease**, **Food Poisoning**, and **Chickenpox**, are **not directly related to air pollution**.
> This indicates that, despite high AQI in several regions, **pollution-linked respiratory conditions are underreported or not captured** in the available health dataset.
> This limits the ability to draw strong correlations between air quality and disease burden in this context.



| State                       | Disease 1               | Count | Disease 2               | Count | Avg AQI |
| --------------------------- | ----------------------- | ----- | ----------------------- | ----- | ------- |
| Andaman and Nicobar Islands | Acute Diarrheal Disease | 3     | Chickenpox              | 1     | 57.71   |
| Andhra Pradesh              | Acute Diarrheal Disease | 89    | Food Poisoning          | 25    | 77.90   |
| Arunachal Pradesh           | Acute Diarrheal Disease | 8     | Chickenpox              | 8     | 54.45   |
| Assam                       | Acute Diarrheal Disease | 88    | Food Poisoning          | 46    | 114.41  |
| Bihar                       | Fever with Rash         | 63    | Acute Diarrheal Disease | 53    | 156.00  |
| Chandigarh                  | Cholera                 | 1     | -                       | -     | 141.13  |
| Chhattisgarh                | Acute Diarrheal Disease | 196   | Food Poisoning          | 19    | 79.08   |
| Delhi                       | Dengue                  | 1     | Measles                 | 1     | 205.13  |
| Gujarat                     | Acute Diarrheal Disease | 88    | Food Poisoning          | 51    | 110.45  |
| Haryana                     | Acute Diarrheal Disease | 14    | Measles                 | 11    | 139.18  |
| Himachal Pradesh            | Acute Diarrheal Disease | 13    | Hepatitis A             | 5     | 160.27  |
| Jammu and Kashmir           | Hepatitis A             | 71    | Mumps                   | 32    | 71.14   |
| Jharkhand                   | Chickenpox              | 94    | Acute Diarrheal Disease | 79    | 164.94  |
| Karnataka                   | Acute Diarrheal Disease | 199   | Food Poisoning          | 85    | 62.51   |
| Kerala                      | Food Poisoning          | 188   | Hepatitis A             | 166   | 68.22   |
| Madhya Pradesh              | Acute Diarrheal Disease | 204   | Dengue                  | 70    | 107.68  |
| Maharashtra                 | Dengue                  | 183   | Acute Diarrheal Disease | 119   | 103.44  |
| Manipur                     | Human Rabies            | 5     | Acute Diarrheal Disease | 4     | 101.25  |
| Meghalaya                   | Human Rabies            | 24    | Measles                 | 18    | 62.89   |
| Mizoram                     | Food Poisoning          | 11    | Acute Diarrheal Disease | 5     | 46.66   |
| Nagaland                    | Dengue                  | 6     | Human Rabies            | 4     | 80.01   |
| Odisha                      | Acute Diarrheal Disease | 229   | Food Poisoning          | 81    | 124.92  |
| Puducherry                  | Acute Diarrheal Disease | 3     | Dengue                  | 3     | 56.94   |
| Punjab                      | Acute Diarrheal Disease | 25    | Chickenpox              | 9     | 117.33  |
| Rajasthan                   | Acute Diarrheal Disease | 19    | Food Poisoning          | 9     | 127.73  |
| Sikkim                      | Typhoid                 | 3     | Acute Diarrheal Disease | 1     | 53.60   |
| Tamil Nadu                  | Mumps                   | 104   | Acute Diarrheal Disease | 84    | 67.96   |
| Telangana                   | Acute Diarrheal Disease | 26    | Food Poisoning          | 7     | 80.47   |
| Tripura                     | Acute Diarrheal Disease | 8     | Acute Gastroenteritis   | 1     | 128.44  |
| Uttar Pradesh               | Acute Diarrheal Disease | 108   | Food Poisoning          | 44    | 124.81  |
| Uttarakhand                 | Acute Diarrheal Disease | 15    | Dengue                  | 7     | 87.80   |
| West Bengal                 | Acute Diarrheal Disease | 76    | Food Poisoning          | 39    | 114.54  |

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

