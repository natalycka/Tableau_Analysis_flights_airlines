# ✈️ U.S. Flight Delays & Cancellations — Tableau Dashboard

An interactive **Tableau** analytics solution exploring U.S. domestic flight performance — delays, cancellations, on-time rates and recovery — across airlines and airports, built on the **U.S. DOT 2015 Flight Delays** dataset.

> Built in Tableau · 2 linked dashboards · 37 worksheets · 52 calculated fields & parameters · Top-N controls · month-over-month trend logic · maps · scatter & butterfly charts.

---

## 🔗 Live dashboard

▶️ **[View it live on Tableau Public](#)** _(replace this link after you publish — see “Publish” below)_

GitHub can't render a `.twbx`, so the **screenshots below** are the static preview and the **Tableau Public link** is the interactive version.

---

## 🧭 Overview

The project turns millions of raw flight records into a decision-oriented analytics system answering:

- How many flights run **on time**, and what share is **delayed (>15 min)** or **cancelled**?
- Which **airlines** and **airports** drive the most delays — and which recover best?
- **Where** (geographically) does departure delay concentrate?
- **Why** are flights delayed or cancelled (weather, carrier, late aircraft, security…)?
- How is average departure delay trending **month over month**?

Two linked dashboards let a stakeholder move from a high-level overview to a deep operational view without losing context.

---

## 🖼️ Dashboard Preview

> Click an image to open it full-size.

### 1. Analysis of Completed Flights — Overview
[![Overview dashboard](screenshots/01-overview.png)](screenshots/01-overview.png)

KPIs (**Total Flights, AVG Departure Delay, Avg Arrival Delay, Cancellation Rate, Delay Rate >15 min**) with sparklines, flight **Status** (On-Time / Delayed / Cancelled) by airline and by departure/arrival airport, and ranked **delay-rate** leaderboards for airlines and large airports. **Top-N** controls and year/airline/airport filters drive the whole page.

### 2. Delay, Recovery & Reasons — Control Panel
[![Control-panel dashboard](screenshots/02-control-panel.png)](screenshots/02-control-panel.png)

KPIs (**Total Airports, Total Airlines, On-Time Performance %, Median Departure Delay**), a **Delay & Recovery** scatter by airline, an **Airport Departure Delay map**, and breakdowns of **cancellation reasons**, **delay reasons** and **on-time vs problem rate** — all driven by a collapsible **Control Panel** (airline filter, month slider, reason legend).

---

## 📊 Dashboards & Key Views

- **KPI headline tiles** with embedded sparklines and trend indicators
- **Stacked bars** — flight status by airline, departure airport and arrival airport
- **Delay-rate leaderboards** — % delayed (>15 min) by airline and by large airports (≥ 3000 flights)
- **Delay & Recovery scatter** — average delay vs recovery by airline
- **Geographic map** — departure delay by airport
- **Butterfly chart** — problem flights vs on-time by airport
- **Reason analysis** — cancellation and delay reasons (weather, air system, carrier, late aircraft, security)
- **Dashboard navigation** — a button to jump between the overview and detail dashboards

---

## 🧮 Calculations & Interactivity (highlights)

**KPIs:** `On-Time Performance %` · `Delay Rate %` · `Delay Rate >15 %` · `Cancellation Rate` · `Median Departure Delay` · `Recovered Delay` · `Problem Rate` / `On-Time Rate`
**Parameters & dynamic controls:** `Top N Airline` · `Top N Airport` (+ Top-N flags) · `Select Bar Metric` → `Bar Metric Selected` (dynamic measure switch) · `Selected Month`
**Time intelligence:** `Avg Departure Delay Current/Previous Month` · `Avg Departure Delay % Change` · `Trend Indicator`
**Classification:** `Flight Status` (On-Time / Delayed / Cancelled) · `Delay > 15 Flag` · `Large Airports (Flights ≥ 3000)` · `Delay Reason` · `Cancellation Reason Name`
**Layout logic:** `Category (Airline / Airport)` · `Orientation` · `Category Type` (butterfly chart) · `Drill Down to City`

_52 calculated fields in total._

---

## ✨ Techniques Demonstrated

- **Parameters** for Top-N filtering and dynamic metric selection
- **Month-over-month** comparison with trend indicators
- **LOD-style aggregations** for rates and recovery metrics
- **Maps**, **scatter plots**, **butterfly charts** and KPI sparklines
- **Dashboard actions & navigation** between linked views
- Custom **layout / control-panel UX** with show-hide containers

---

## 🧰 Tools & Technologies

`Tableau Desktop` · `Tableau Public` · `Calculated Fields` · `Parameters` · `LOD expressions` · `Data Visualization` · `Dashboard design`

---

## 📂 Dataset

**U.S. DOT — 2015 Flight Delays and Cancellations** (14 U.S. carriers), available on Kaggle:
<https://www.kaggle.com/datasets/usdot/flight-delays>
A reduced working extract (`flights_light`) is packaged inside the `.twbx`.

---

## ▶️ Explore the workbook

- **Interactive:** open the Tableau Public link above.
- **Local:** download **`flight_delays_dashboard.twbx`** and open it in **[Tableau Public Desktop](https://www.tableau.com/products/public)** (free) or Tableau Desktop. The data extract is packaged inside the file.

### How to publish on Tableau Public
1. Open the `.twbx` in Tableau Public Desktop.
2. **Server → Tableau Public → Save to Tableau Public** (create a free account).
3. Copy the published URL and paste it into the **Live dashboard** link at the top of this README.

---

## 👩‍💻 Author

**Nataliia Savenko** — Data Analyst, Nuremberg, Germany
📧 nsavenko82@gmail.com · 💼 [LinkedIn](https://www.linkedin.com/in/nataliia-s-3b1a6178/)
