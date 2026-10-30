# C++ Search-and-Rescue Swarm Drone Simulation

An interactive 2D simulation of an autonomous swarm of drones performing search-and-rescue operations in an obstacle-filled environment.

Developed in **C++**, the project explores swarm coordination, autonomous navigation, spatial dispersion, and resource management. It features a custom swarm behaviour algorithm, a desktop graphical interface built with **wxWidgets**, and real-time 2D visualization powered by **gnuplot**.

## Features

### Autonomous Swarm Intelligence
- **Biased Random Walk:** Drones use a biased random walk to explore the environment while maintaining spatial dispersion.
- **Inter-Drone Repulsion:** A repulsion mechanism encourages drones to maintain separation, reducing clustering and potential collisions.
- **Obstacle Avoidance:** Drones account for obstacles when navigating the search environment.

### Search-and-Rescue Operations
- **Survivor Detection:** Drones detect survivors within their active scanning radius.
- **Dynamic Rescue Mechanism:** Detected survivors are rescued and tracked throughout the simulation.
- **Spatial Tracking:** Visited map regions are recorded to monitor search coverage and exploration progress.

### Battery Management
- **Dynamic Power Consumption:** Battery levels decrease according to drone flight speed.
- **Battery Monitoring:** Individual drone battery levels are tracked throughout the simulation.
- **Automatic Deactivation:** Drones stop operating when their batteries are depleted.

### Interactive Graphical Interface
- **wxWidgets GUI:** A desktop interface provides interactive control over simulation parameters.
- **Dynamic Configuration:** Adjust the number of active drones and survivor targets using sliders.
- **Real-Time Visualization:** Observe drone movement, search coverage, obstacles, and survivor locations through a live 2D plot.

### Live 2D Visualization
- **gnuplot Integration:** Simulation data is piped directly to a gnuplot process for real-time rendering.
- **Trajectory Tracking:** Visualizes individual drone movement and exploration paths.
- **Search Radius Display:** Shows the active scanning radius of each drone.
- **Environment Mapping:** Displays obstacles, survivor positions, and explored regions.

## Project Structure

```text
CPP-Drone-Search/
├── include/                  # Header files
│   ├── Drone.h               # Swarm drone class definition
│   ├── Map.h                 # 2D environment and grid management
│   └── MyFrame.h             # wxWidgets main frame and gnuplot interface
│
├── src/                      # Implementation files
│   ├── Drone.cpp             # Movement, repulsion and scanning logic
│   ├── Map.cpp               # Obstacle/survivor generation and spatial tracking
│   ├── MyFrame.cpp           # GUI event handlers and visualization pipeline
│   ├── main.cpp              # Application entry point
│   └── myapp.rc              # Windows resource script
│
├── Cpluplus_Projecct.cbp     # Code::Blocks project file
├── .gitignore                # Git exclusion settings
└── README.md                 # Project documentation
```

## Technologies Used

| Technology | Application |
|---|---|
| **C++** | Core simulation logic and swarm behaviour |
| **wxWidgets** | Desktop graphical user interface |
| **gnuplot** | Real-time 2D visualization |
| **Code::Blocks** | Project configuration and development environment |

## Core Concepts

This project explores several concepts relevant to autonomous robotics and multi-agent systems:

- **Swarm Robotics:** Coordinated behaviour emerging from interactions between multiple autonomous agents.
- **Randomized Exploration:** Biased random walks for decentralized environmental exploration.
- **Collision Avoidance:** Inter-agent repulsion and obstacle avoidance.
- **Search Coverage:** Spatial tracking and exploration of an unknown environment.
- **Resource Management:** Battery-aware autonomous operation.
- **Real-Time Visualization:** Dynamic representation of multi-agent behaviour and simulation states.

## Potential Future Improvements

- Implement more advanced swarm coordination and decentralized exploration strategies.
- Introduce adaptive search patterns based on previously explored regions.
- Develop more sophisticated path planning and obstacle avoidance algorithms.
- Implement dynamic battery-aware task allocation and return-to-base behaviour.
- Introduce communication and information-sharing mechanisms between drones.
- Extend the simulation from 2D to a 3D environment.

## Project Objective

The project aims to explore how multiple autonomous agents can cooperate to perform search-and-rescue operations in an environment containing obstacles and distributed targets.

By combining decentralized exploration, inter-agent coordination, survivor detection, and battery management, the simulation demonstrates fundamental principles of swarm robotics and autonomous multi-agent systems.
