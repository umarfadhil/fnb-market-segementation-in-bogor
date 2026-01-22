# FnB Market Segmentation in Bogor 🍜📍

This project analyzes the Food & Beverage (FnB) market in **Kota Bogor** to uncover hidden patterns across **areas**, **categories**, and **customer value** using data-driven segmentation techniques.

Portfolio page: **petalytix.id/en/portfolio/fnb-market-segmentation-in-bogor**

---

## Why this exists

If you’re a business owner, investor, or city planner, “FnB is growing” isn’t actionable. This project turns location data into decisions like:

- Which areas are **over-saturated vs under-served**?
- Which areas likely contain **higher value customers** (proxy: willingness-to-pay (WTP) / price signals)?
- What **market segments** exist in Bogor, and how do they differ spatially?

---

## What you’ll find in this repo

- **`FnB_Market_Segmentation_in_Bogor.ipynb`** — main analysis notebook (data prep → feature engineering → clustering → profiling → mapping).
- **`bogor_fnb_map.html`** — interactive map output (clusters / WTP-style layers).

---

## Approach (high level)

1. **Collect & clean location-based FnB data from Google Maps** (e.g., categories, coordinates, popularity proxies, and price/WTP signals if available).
2. **Feature engineering**  
   Examples of useful signals:
   - Category mix (and diversity/balance)
   - Density / saturation by area
   - Popularity signals (ratings/reviews, if present)
   - Price / WTP proxy signals (if present)
3. **Unsupervised segmentation**
   - Cluster areas/outlets to discover “types” of markets
4. **Cluster profiling**
   - Turn cluster IDs into human-readable segments
5. **Spatial visualization**
   - Map clusters (colored markers)
   - Overlay WTP-style intensity (heatmap) and optionally filter by category

---

## How to run

### Option A — Run the notebook locally

1. **Clone**
   ```bash
   git clone https://github.com/umarfadhil/fnb-market-segementation-in-bogor.git
   cd fnb-market-segementation-in-bogor

2. **Create env**
   python -m venv .venv
   # Windows:
   .\.venv\Scripts\activate
   # Mac/Linux:
   source .venv/bin/activate

3. **Install dependencies**
   pip install -U pip
   pip install pandas numpy scikit-learn matplotlib folium jupyter

4. **Open Jupyter**
   jupyter notebook

### Option B — View the interactive map

Open bogor_fnb_map.html
