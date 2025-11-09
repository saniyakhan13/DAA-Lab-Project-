# DAA-Lab-Project-
# Emergency Vehicle Allocation System using Dijkstra’s Algorithm

This project is a **Python 3 application** designed to efficiently locate and assign the **nearest available emergency vehicle** based on the requester’s zip code.  
It uses **Dijkstra’s algorithm** to compute the **shortest route** between locations, ensuring quick response times during emergencies.

---

## Project Overview
Whenever an emergency request is raised, the system identifies the **closest available vehicle** by:
1. Mapping all vehicle and request locations as graph nodes.
2. Using **Dijkstra’s algorithm** to determine the shortest distance between the source (request location) and all destinations.
3. Allocating the **nearest available emergency vehicle** to the requester.

This helps optimize dispatch time and improve emergency response efficiency.

---

## Technologies Used
- **Python 3**
- **NetworkX** (for graph representation and shortest path computation)
- **Matplotlib** (optional visualization)
- **Pandas / CSV** (for location and vehicle data storage)

---

## How It Works
1. Each location (zip code) is treated as a node in a weighted graph.
2. Edges represent the distances or travel times between nearby locations.
3. When a new request arrives:
   - The system runs **Dijkstra’s algorithm** from the request’s zip code.
   - Finds the **shortest path** to all vehicle locations.
   - Chooses the **closest available vehicle**.
4. Once a vehicle is assigned, it is marked as **busy** until it becomes available again.

---

## Algorithm Explanation
**Dijkstra’s Algorithm** works by exploring all possible paths from a starting node and always choosing the path with the lowest total distance so far.  
It guarantees the **shortest path** to every other node in a weighted graph where all edges have non-negative weights.

---

## Future Improvements
- Integrate **real-time GPS data** for live vehicle tracking.
- Add a **web interface** for visual route display.
- Include **vehicle type and capacity matching** for advanced dispatch logic.

---

## Author
Saniya Intezar Khan 
