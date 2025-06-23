# Logistic-Portfolio
Logistics projects that illustrate my ability to analyze and interpret both exploratory and geographic data for real-world insights.

# Geographical Service Area Optimization

This project visualizes and analyzes service area definitions for five logistics hubs using customer location data, postal code boundaries, and Google MyMaps. It serves as the foundation for further routing and coverage optimizations.

---

## 📌 Project Objectives | Business Questions

- Define optimal service areas per logistics hub.
- Identify geographical overlaps or inefficiencies.
- Visualize customer distribution and service coverage.
- Serve as a basis for planning workload allocation and travel times.

---

## 📊 Summary of Insights

- Five distinct catchment areas were derived based on real customer locations.
- Spatial clusters aligned well with postal code regions and travel times.
- Overlapping zones and outliers were visually identified and can be reallocated to improve efficiency.

---

## ✅ Recommendations and Next Steps

- Assign boundary zones based on travel time thresholds (e.g., max 90 minutes).
- Reallocate edge customers to balance workload between hubs.
- Use these maps for driver shift planning and route simulations (→ see next project).
- Integrate with routing tools (e.g., GraphHopper, OpenRouteService) to calculate travel time isochrones.

---

## 🗂 General Information

- Tools used: Google MyMaps, Excel/CSV, public PLZ shapefiles ([OpenDataSoft source](https://public.opendatasoft.com/explore/dataset/georef-germany-postleitzahl/map/)).
- Data: Customer locations from internal CRM (anonymized), postal code boundaries (KML).
- Output: Interactive map and this static visual export.

### 📍 Visual Output 

![Service Area Map](./d4af1af4-dd5d-4804-8f0e-f842a2079320.pn)

> [View Full Interactive Map](https://www.google.com/maps/d/u/0/edit?mid=1lmA6G2OOP2aNDyRpng9ZkhoNyPqnxJo&ll=52.15407456290242%2C14.042294269756827&z=9)

---


