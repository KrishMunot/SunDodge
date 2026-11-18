# SunDodge 🏙️🚶‍♂️

**Walk Dubai without melting.** SunDodge is a routing app that finds walking paths with maximum shade based on real-time sun position and 3D building shadows.

## Why SunDodge?
Standard navigation apps optimize for the shortest distance or fastest time. In Dubai, a 2-minute shorter walk in direct sunlight can feel like an eternity. SunDodge trades a few extra steps for maximum shadow coverage.

## Key Features
- **Shade-First Routing:** Prioritizes sidewalks and paths covered by building shadows over the absolute shortest route.
- **Time-Aware Shadows:** Dynamically adjusts routes based on the current time of day and solar azimuth/elevation.
- **Shade vs. Distance Trade-off:** Compare the fastest route against the shadiest route (e.g., *+3 mins walk, +65% shade*).
- **Dubai-Focused:** Built around high-density urban corridors where skyscraper shadows make a real difference.

## How It Works *(Planned Architecture)*
1. **3D Building Data:** Pulls building footprints and heights (e.g., OpenStreetMap / Overture Maps).
2. **Solar Calculation:** Computes sun angle (altitude & azimuth) for the requested date and time.
3. **Shadow Projection:** Projects building shadow polygons onto the pedestrian street graph.
4. **Weighted Routing:** Runs pathfinding (A* / Dijkstra) with edge weights penalized by sun exposure.

## Getting Started
*Coming soon — project is currently in active development.*

```bash
git clone [https://github.com/KrishMunot/SunDodge.git](https://github.com/KrishMunot/SunDodge.git)
cd SunDodge
