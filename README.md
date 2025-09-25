# 🚇 Meto Mate – Efficient Metro Route Planner

Meto Mate is a **C++ project** designed to help commuters in Indian cities (Delhi, Bangalore, Hyderabad) find the **shortest, cheapest, and most convenient routes** across metro networks.  
This project was developed as part of the **DSA-II Course Project** at NIT Karnataka.

---

## 📌 Features
- **Shortest Travel Time** – Uses Dijkstra’s Algorithm to compute the fastest path.  
- **Minimum Fare Path** – Optimizes for cost-effective travel.  
- **Fewest Interchanges** – BFS with line tracking to minimize station changes.  
- **Scalable Design** – Easily expandable to new cities and metro lines.  
- **Error Handling** – Handles missing stations, invalid inputs, and unreachable destinations.

---

## 🏗️ Motivation
- Cities like **Delhi & Bangalore** are among the most traffic-congested in India.  
- Commuters struggle with finding optimal metro routes based on time, fare, and interchanges.  
- This project encourages **public transport usage**, helping reduce **traffic congestion, pollution, and travel stress**.  
- Designed to provide an **accessible, efficient, and scalable solution** using **graph algorithms**.

---

## ⚙️ Implementation
- **Language:** C++  
- **Algorithms Used:**
  - *Dijkstra’s Algorithm* → Shortest/cheapest route (O((V + E) log V))  
  - *BFS with deque* → Fewest interchanges (O(V + E))  
- **Graph Representation:** Adjacency List  
  - Nodes → Metro Stations  
  - Edges → Connections (with attributes: time, distance, cost, line color)  
- **Data Files:**
  - `stations.txt` → Station IDs & names  
  - `connections.txt` → Routes with distance, time, and fare  

Example Compilation:
```bash
g++ main.cpp delhi/delhi.cpp bangalore/bangalore.cpp hyderabad/hyderabad.cpp inter-city/inter-city.cpp -o meto_mate
./meto_mate
