# 🏨 Hotel Booking Demand — Exploratory Data Analysis (EDA)

This project performs an end-to-end Exploratory Data Analysis (EDA) on a 
real-world hotel bookings dataset containing **119,390 bookings** across 
**City Hotel** and **Resort Hotel** from 2015 to 2017. The goal is to uncover 
booking patterns, guest behavior, pricing trends, and cancellation drivers 
that can help hospitality businesses make data-driven decisions.

---

## 📊 Data

| Property | Details |
|----------|---------|
| **Dataset** | Hotel Booking Demand |
| **Source** | [Kaggle — Jesse Mostipak](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand) |
| **File** | hotel_bookings.csv |
| **Rows** | 119,390 |
| **Columns** | 32 |
| **Time Period** | July 2015 — August 2017 |
| **Hotel Types** | City Hotel, Resort Hotel |

### Key Columns Used
- `hotel` — Hotel type (City Hotel / Resort Hotel)
- `is_canceled` — Whether booking was cancelled (1) or not (0)
- `country` — Guest country of origin
- `arrival_date_month` — Month of arrival
- `adr` — Average Daily Rate (price per night in €)
- `reserved_room_type` — Room type reserved
- `meal` — Meal plan chosen
- `market_segment` — Booking channel
- `total_of_special_requests` — Number of special requests made
- `stays_in_weekend_nights` + `stays_in_week_nights` — Length of stay

---

## 🔍 Data Contact

- **Chaithanya AS** — [your-email@gmail.com] — Contact for inquiries regarding 
  this analysis and dataset usage.
- **Original Dataset** — Available publicly on Kaggle (no expiration).
- Data is used strictly for educational and analytical purposes.

---

## 🚀 Getting Started

### Primary Analysis Script
Open and run the Jupyter Notebook:
```
Hotel_Booking_EDA.ipynb
```
Run all cells sequentially from top to bottom.

---

## ⚙️ Requirements

### Step 1 — Clone the Repository
```bash
git clone https://github.com/YOUR_USERNAME/hotel-booking-eda.git
cd hotel-booking-eda
```

### Step 2 — Install Dependencies
```bash
pip install pandas numpy matplotlib seaborn plotly jupyter
```

### Step 3 — Launch Jupyter Notebook
```bash
jupyter notebook
```

### Step 4 — Open and Run
```
Open Hotel_Booking_EDA.ipynb
Run all cells (Cell → Run All)
```

### Step 5 — Example Output
```python
# Sample output from Cell 2
Shape: (119390, 32)

# Sample output from Cell 13
Total Bookings: 119386
Cancelled: 44217
Cancellation Rate: 37.04%
```

---

## 📋 Analysis Structure

### Part A — Data Understanding & Cleaning
- Loaded and inspected dataset (shape, dtypes, missing values, duplicates)
- Handled missing values in `children`, `country`, `agent`, `company`
- Removed invalid ADR values (negative or > 5000)
- Created derived features: `total_nights`, `total_guests`
- Built a clean non-cancelled bookings dataset (`df_clean`)

### Part B — Core EDA Questions Answered

| # | Question | Method |
|---|----------|--------|
| 1 | Where do guests come from? | Bar chart + World Choropleth Map |
| 2 | How much do guests pay per night? | Box plot + Bar chart (ADR) |
| 3 | How does price vary across the year? | Line chart (monthly ADR) |
| 4 | What are guest meal preferences? | Bar chart + Percentage table |
| 5 | Special requests vs cancellations? | Bar chart + Pivot table |
| 6 | Which months are busiest? | Line chart (monthly volume) |
| 7 | Length of stay analysis | Histogram + KDE |
| 8 | Market segment analysis | Bar chart + ADR comparison |
| 9 | Cancellation analysis | Bar charts by hotel and month |

---

## 💡 Key Insights

- 🌍 **Portugal (PRT)** is the top guest origin country with **17,662 bookings**, 
  followed by UK (8,447) and France (7,184) — European guests dominate.

- 💰 **City Hotel charges more** — Average ADR of **€108.28/night** vs 
  Resort Hotel at **€92.97/night**.

- 📅 **August is the busiest month** for both hotels AND has the highest 
  cancellation rate of **32.2%** — peak season paradox!

- 🍳 **Bed & Breakfast (BB)** is the most popular meal plan — chosen by 
  **~79% of guests** in both City and Resort hotels.

- 🌐 **Online Travel Agents (OTA)** bring the highest number of bookings, 
  but Direct bookings command higher ADR.

- ❌ **0 special requests = highest cancellation** — Guests who make more 
  special requests are significantly less likely to cancel their booking.

- 🛏️ **Resort Hotel guests stay longer** than City Hotel guests — 
  Resort is preferred for leisure, City for short business trips.

---

## 🛠️ Tools Used

| Tool | Purpose |
|------|---------|
| Python 3.11 | Programming language |
| Pandas | Data manipulation and analysis |
| NumPy | Numerical computations |
| Matplotlib | Static visualizations |
| Seaborn | Statistical visualizations |
| Plotly | Interactive world map choropleth |
| Jupyter Notebook | Development environment |

---

## 📁 Project Structure

```
HotelEDA/
├── Hotel_Booking_EDA.ipynb    ← Main analysis notebook
├── hotel_bookings.csv         ← Dataset
├── hotel_eda_dashboard.png    ← Summary dashboard image
└── README.md                  ← This file
```

---

## 👤 Author

**Chaithanya AS**
- MCA Student — Amrita Vishwa Vidyapeetham
- GitHub: [chaithanya-sunil](https://github.com/chaithanya-sunil)
- Email: chaithanyasunil607@gmail.com

---

## 🙏 Acknowledgments

- Dataset originally published by **Antonio, Almeida and Nunes (2019)** — 
  *Hotel booking demand datasets*, Data in Brief.
- Dataset made available on Kaggle by Jesse Mostipak.
- Project inspired by UnsaidTalks Data Analyst program.

---

## 📄 License

This project is licensed under the **MIT License** — 
free to use for educational purposes with attribution.

---

*Submitted as part of UnsaidTalks Data Analyst EDA Assignment — 2025*
