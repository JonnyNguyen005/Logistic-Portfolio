# Economic Reachability Zones via Travel-Time Isochrones

This project visualizes economically viable dispatch areas for five disposal service hubs in Brandenburg. Using realistic road network travel times, the map shows which areas can be reached within a practical time budget, accounting for outbound trip, customer interaction, and return.

---

## 📌 Project Objectives | Business Questions

- What is the maximum cost-effective dispatch radius from each location?
- Which areas can be reached, serviced, and returned from within a standard work shift?
- How do topography and routing conditions influence operational planning?

---

## 📊 Summary of Insights

- Each isochrone represents the **maximum area reachable in 60 minutes one-way**, based on road conditions.
- Field knowledge (e.g., "Frankfurt/Oder → Berlin not profitable") aligns with model outputs.
- Economic zones are **not circular** but based on **actual street network travel times**.

---

## 🔧 Assumptions & Parameters

| Component                        | Assumption / Value                             |
|----------------------------------|-----------------------------------------------|
| Total job duration per shift     | 8.5 hours                                     |
| Time spent on-site per customer  | 5–30 minutes (avg. 20 min used)               |
| Buffer for congestion, wait time | ~30–45 minutes                                |
| Remaining time for driving       | ~8.0 hours                                    |
| One-way trip allowance           | 3.5–4.0 hours                                 |
| Avg. net driving speed           | 45–50 km/h (includes local delays)            |
| Derived range (1 direction)      | ~160–180 km (→ not shown as air radius)       |
| Routing engine                   | OpenRouteService (ORS) API                    |
| API profile                      | `driving-car` (free tier)                     |
| Max range shown per site         | **3600 seconds = 60 minutes driving**         |
| Map type                         | Isochrones via real routing – not geometric   |
| Return trip included?            | **No** – map shows outbound travel only       |

---

## ✅ Recommendations and Next Steps

- Treat displayed zones as **economic boundaries for one-way dispatch**.
- Do not serve customers outside these zones unless route bundling or high-margin jobs justify it.
- Add customer location overlays and value tiers for dispatch prioritization.
- Upgrade to `driving-hgv` profile or custom routing if LKW-specific factors are critical.

---

## 🗂 General Information

- Tools: Leaflet.js + OpenRouteService API
- Routing profile: `driving-car`
- Time range: 60 minutes per location
- Locations:
  - Frankfurt (Oder)
  - Fürstenwalde
  - Eisenhüttenstadt
  - Ludwigsfelde
  - Kolkwitz (Krieschow)

---

### 📍 Visual Output 

![60-Min Isochrone Map](https://github.com/user-attachments/assets/08050223-d3ec-4e4f-b406-0287d5426feb)


> Each color-coded zone shows the area reachable from a site within 60 minutes of realistic driving time — excluding return trip or on-site time.

---
