# 🏨 Hotel Booking Analysis

## 📌 Overview
The **Hotel Booking Analysis** project aims to explore and analyze hotel booking data to uncover key patterns and insights that can help improve customer satisfaction and business efficiency.  
The analysis focuses on understanding factors influencing cancellations, booking trends, customer demographics, and seasonal behaviors.

---

## 📂 Dataset Description
The dataset used for this project is **`hotel_booking.csv`**, which contains details about bookings made for two types of hotels — **City Hotel** and **Resort Hotel**.

### Key Columns:
- `hotel`: Type of hotel (City or Resort)
- `is_canceled`: Whether the booking was canceled (1) or not (0)
- `lead_time`: Number of days between booking and arrival
- `arrival_date_month`: Month of arrival
- `stays_in_weekend_nights`: Number of weekend nights spent
- `stays_in_week_nights`: Number of week nights spent
- `adults`, `children`, `babies`: Number of guests
- `meal`: Type of meal booked
- `country`: Country of origin
- `market_segment`: Type of booking (e.g., Online TA, Offline TA)
- `reserved_room_type`: Room category reserved
- `reservation_status_date`: Date of reservation status update
- `deposit_type`: Type of deposit made
- `customer_type`: Type of customer (Transient, Group, etc.)

---

## 🧹 Data Preprocessing
1. Loaded the dataset using **Pandas**.
2. Checked for missing values using `isnull().sum()`.
3. Dropped unnecessary columns like `company` and `agent`.
4. Converted the column `reservation_status_date` to a datetime format.
5. Removed rows with missing values using `dropna()`.

---

## 📊 Exploratory Data Analysis (EDA)
EDA was performed using **Seaborn** and **Matplotlib** to visualize patterns such as:
- Booking trends over time
- Cancellation rates by hotel type
- Average lead time distribution
- Country-wise booking statistics
- Effect of deposit type on cancellations
- Seasonal booking behavior

### Example Visualizations:
- `sns.countplot()` for hotel type vs. cancellations
- `sns.heatmap()` for correlation matrix
- `plt.hist()` for lead time and stay duration

---

## 🧠 Insights & Findings
- **City Hotels** experience higher cancellation rates than Resort Hotels.
- Most bookings are made through **Online Travel Agencies**.
- Longer lead times are more likely to result in cancellations.
- Bookings from certain countries dominate the dataset.
- Seasonal demand shows peaks during **summer months**.
- Customers with **no deposits** have higher cancellation tendencies.

---

## 🧰 Technologies & Libraries Used
- **Python 3**
- **NumPy**
- **Pandas**
- **Matplotlib**
- **Seaborn**
- **Scikit-learn**

---

## ⚙️ How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/SatyanarayanaG2908/Hotel-Booking-Analysis
   cd Hotel-Booking-Analysis
