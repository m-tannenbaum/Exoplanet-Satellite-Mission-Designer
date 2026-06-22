# Exoplanet Satellite Mission Designer

A MATLAB tool for designing and visualizing satellite missions around 
exoplanets, inspired by real aerospace engineering and exoplanet research.

![Earth Mission](Screenshots/Earth%20Mission%20Screenshot.png)
![TOI-1347b Mission](Screenshots/TOI-1347b%20Mission%20Screenshot.png)

---

## Background

This project grew out of several converging interests, such as watching satellite 
builds and assemblies at Northrop Grumman, researching the exoplanet TOI-1347b 
with the STEPUP group at Pitt, and studying missions like NASA's ESCAPADE and 
SpaceX's Starlink constellation. The goal was to build something that combined 
orbital mechanics, real exoplanet data, and mission planning into one tool.

---

## Features

- User interactive mission designer with planet and orbit selection
- Three planet modes: Earth, TOI-1347b (real exoplanet), and Custom
- User-defined orbital parameters: altitude, eccentricity, speed multiplier
- Real-time satellite telemetry HUD
- Mission analysis panel with orbital mechanics calculations
- Four-check mission viability system with GO/NO-GO status
- 3D animated satellite with solar panels orbiting a textured planet
- Multi-layer atmospheric glow per planet
- Depth-varied starfield with 2500 stars

---

## Physics

- Newton's Law of Gravitation
- Vis-Viva Equation for live orbital velocity
- Kepler's Third Law for orbital period
- Roche Limit (rigid body approximation)
- Elliptical orbit via true anomaly
- Delta-V to escape from orbit

---

## Mission Viability Checks

| Check | Condition |
|---|---|
| Roche Clearance | Periapsis > Roche limit × 1.1 |
| Min Orbital Period | Period > 1 hour |
| Escape Velocity | Orbital velocity < escape velocity |
| Altitude Safety | Periapsis altitude > 100 km |

---

## How to Run

1. Open `Exoplanet_Mission_Designer` in MATLAB
2. Place planet texture images in the same folder
3. Run the script, and the mission designer dialogs will appear
4. Select planet, set orbital parameters, and launch

---

## Planet Modes

| Planet | Radius | Mass | Rotation Period |
|---|---|---|---|
| Earth | 1.0 R⊕ | 1.0 M⊕ | 24 hr |
| TOI-1347b | 1.8 R⊕ | 11.1 M⊕ | 20.3 hr |
| Custom | User defined | User defined | User defined |

---

## Inspiration

- Northrop Grumman - satellite hardware and systems engineering
- STEPUP at Pitt - exoplanet observation and TOI-1347b research  
- NASA ESCAPADE - twin satellite Mars mission architecture
- SpaceX Starlink - large constellation orbital design

---

## Author

Matthew Tannenbaum  
Electrical Engineering, Physics & Astronomy - University of Pittsburgh  
EE Intern @ Northrop Grumman | Electronic Systems & Astrophysics Researcher | Honors EE + Physics & Astronomy Student
