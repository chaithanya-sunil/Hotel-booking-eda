\# 🏨 Hotel Booking Demand — Exploratory Data Analysis (EDA)



This project performs an end-to-end Exploratory Data Analysis (EDA) on a 

real-world hotel bookings dataset containing \*\*119,390 bookings\*\* across 

\*\*City Hotel\*\* and \*\*Resort Hotel\*\* from 2015 to 2017. The goal is to uncover 

booking patterns, guest behavior, pricing trends, and cancellation drivers 

that can help hospitality businesses make data-driven decisions.



\---



\## 📊 Data



| Property | Details |

|----------|---------|

| \*\*Dataset\*\* | Hotel Booking Demand |

| \*\*Source\*\* | \[Kaggle — Jesse Mostipak](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand) |

| \*\*File\*\* | hotel\_bookings.csv |

| \*\*Rows\*\* | 119,390 |

| \*\*Columns\*\* | 32 |

| \*\*Time Period\*\* | July 2015 — August 2017 |

| \*\*Hotel Types\*\* | City Hotel, Resort Hotel |



\### Key Columns Used

\- `hotel` — Hotel type (City Hotel / Resort Hotel)

\- `is\_canceled` — Whether booking was cancelled (1) or not (0)

\- `country` — Guest country of origin

\- `arrival\_date\_month` — Month of arrival

\- `adr` — Average Daily Rate (price per night in €)

\- `reserved\_room\_type` — Room type reserved

\- `meal` — Meal plan chosen

\- `market\_segment` — Booking channel

\- `total\_of\_special\_requests` — Number of special requests made

\- `stays\_in\_weekend\_nights` + `stays\_in\_week\_nights` — Length of stay



\---



\## 🔍 Data Contact



\- \*\*Chaithanya AS\*\* — \[your-email@gmail.com] — Contact for inquiries regarding 

&#x20; this analysis and dataset usage.

\- \*\*Original Dataset\*\* — Available publicly on Kaggle (no expiration).

\- Data is used strictly for educational and analytical purposes.



\---



\## 🚀 Getting Started



\### Primary Analysis Script

Open and run the Jupyter Notebook:

```

Hotel\_Booking\_EDA.ipynb

```

Run all cells sequentially from top to bottom.



\---



\## ⚙️ Requirements



\### Step 1 — Clone the Repository

```bash

git clone https://github.com/YOUR\_USERNAME/hotel-booking-eda.git

cd hotel-booking-eda

```



\### Step 2 — Install Dependencies

```bash

pip install pandas numpy matplotlib seaborn plotly jupyter

```



\### Step 3 — Launch Jupyter Notebook

```bash

jupyter notebook

```



\### Step 4 — Open and Run

```

Open Hotel\_Booking\_EDA.ipynb

Run all cells (Cell → Run All)

```



\### Step 5 — Example Output

```python

\# Sample output from Cell 2

Shape: (119390, 32)



\# Sample output from Cell 13

Total Bookings: 119386

Cancelled: 44217

Cancellation Rate: 37.04%

```



\---



\## 📋 Analysis Structure



\### Part A — Data Understanding \& Cleaning

\- Loaded and inspected dataset (shape, dtypes, missing values, duplicates)

\- Handled missing values in `children`, `country`, `agent`, `company`

\- Removed invalid ADR values (negative or > 5000)

\- Created derived features: `total\_nights`, `total\_guests`

\- Built a clean non-cancelled bookings dataset (`df\_clean`)



\### Part B — Core EDA Questions Answered



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



\---



\## 💡 Key Insights



\- 🌍 \*\*Portugal (PRT)\*\* is the top guest origin country with \*\*17,662 bookings\*\*, 

&#x20; followed by UK (8,447) and France (7,184) — European guests dominate.



\- 💰 \*\*City Hotel charges more\*\* — Average ADR of \*\*€108.28/night\*\* vs 

&#x20; Resort Hotel at \*\*€92.97/night\*\*.



\- 📅 \*\*August is the busiest month\*\* for both hotels AND has the highest 

&#x20; cancellation rate of \*\*32.2%\*\* — peak season paradox!



\- 🍳 \*\*Bed \& Breakfast (BB)\*\* is the most popular meal plan — chosen by 

&#x20; \*\*\~79% of guests\*\* in both City and Resort hotels.



\- 🌐 \*\*Online Travel Agents (OTA)\*\* bring the highest number of bookings, 

&#x20; but Direct bookings command higher ADR.



\- ❌ \*\*0 special requests = highest cancellation\*\* — Guests who make more 

&#x20; special requests are significantly less likely to cancel their booking.



\- 🛏️ \*\*Resort Hotel guests stay longer\*\* than City Hotel guests — 

&#x20; Resort is preferred for leisure, City for short business trips.



\---



\## 🛠️ Tools Used



| Tool | Purpose |

|------|---------|

| Python 3.11 | Programming language |

| Pandas | Data manipulation and analysis |

| NumPy | Numerical computations |

| Matplotlib | Static visualizations |

| Seaborn | Statistical visualizations |

| Plotly | Interactive world map choropleth |

| Jupyter Notebook | Development environment |



\---



\## 📁 Project Structure



```

HotelEDA/

├── Hotel\_Booking\_EDA.ipynb    ← Main analysis notebook

├── hotel\_bookings.csv         ← Dataset

├── hotel\_eda\_dashboard.png    ← Summary dashboard image

└── README.md                  ← This file

```



\---



\## 👤 Author



\*\*Chaithanya AS\*\*

\- MCA Student — Amrita Vishwa Vidyapeetham

\- GitHub: \[chaithanya-sunil](https://github.com/chaithanya-sunil)

\- Email: chaithanyasunil607@gmail.com



\---



\## 🙏 Acknowledgments



\- Dataset originally published by \*\*Antonio, Almeida and Nunes (2019)\*\* — 

&#x20; \*Hotel booking demand datasets\*, Data in Brief.

\- Dataset made available on Kaggle by Jesse Mostipak.

\- Project inspired by UnsaidTalks Data Analyst program.



\---



\## 📄 License



This project is licensed under the \*\*MIT License\*\* — 

free to use for educational purposes with attribution.



\---



\*Submitted as part of UnsaidTalks Data Analyst EDA Assignment — 2025\*



