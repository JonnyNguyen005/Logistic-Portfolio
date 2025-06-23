# Economic Reachability Zones via Travel-Time Isochrones

This project visualizes the economically viable service areas for five disposal hubs based on real road travel time. It uses isochrone data to identify which zones can be served within a 60-minute drive — the typical upper threshold for cost-efficient operations in single-stop disposal services.

---

## 📌 Project Objectives | Business Questions

- What is the realistic reach for a vehicle from each location within 1 hour of driving?
- How do these zones differ across locations?
- Where are overlaps, white spots, or marginal areas?

---

## 📊 Summary of Insights

- All five sites show clear service boundaries when constrained to 60 minutes travel time.
- The map highlights regional service gaps and overlaps.
- Several economically marginal areas like Berlin (from Frankfurt Oder) fall outside feasible zones.

---

## ✅ Recommendations and Next Steps

- Limit dispatch radius to 45–60 minutes driving time per vehicle.
- Avoid areas outside the red zones unless combined with multi-stop routes.
- Use time-based zones instead of circles for realistic territory planning.
- Integrate customer locations and order value to optimize routing further.

---

## 🗂 General Information

- Tools: Leaflet.js + OpenRouteService Isochrone API
- Routing profile: `driving-car` (due to free tier limits)
- Time range: 60 minutes (3600 seconds)
- Locations:
  - Frankfurt (Oder)
  - Fürstenwalde
  - Eisenhüttenstadt
  - Ludwigsfelde
  - Kolkwitz (Krieschow)

### 📍 Visual Output (Preview)

![Isochrone Map (Simplified)](./isochronen_maxfahrtzeit_standortfarben.png)

> *Each location has a single time-based reachability zone, color-coded and overlaid for comparison.*

---

