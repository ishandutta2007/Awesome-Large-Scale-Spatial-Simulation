# Awesome Large-Scale Spatial Simulation Ecosystem

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![Tracked Projects](https://img.shields.io/badge/Projects-20%2B-blue?style=flat-square)](https://github.com/ishandutta2007/Awesome-Large-Scale-Spatial-Simulation)

> A curated directory of enterprise SaaS platforms and top open-source engines for **large-scale spatial simulation**, **city-scale digital twins**, **agent-based modeling (ABM)**, **autonomous vehicle testing**, and **geospatial 3D visualization**.

---

## Table of Contents
- [Market Overview & Ecosystem Dynamics](#market-overview--ecosystem-dynamics)
- [Commercial & Enterprise SaaS Platforms](#commercial--enterprise-saas-platforms)
- [Top Open-Source Spatial Simulation Engines](#top-open-source-spatial-simulation-engines)
- [Framework Integration & Architecture Patterns](#framework-integration--architecture-patterns)
- [How to Contribute](#how-to-contribute)
- [Disclaimer & License Notes](#disclaimer--license-notes)

---

## Market Overview & Ecosystem Dynamics

**Estimated Market Size**: The global **Spatial Simulation and Digital Twin Market** is valued at **~$18.4 Billion in 2026** and is projected to reach **~$85 Billion by 2032**, growing at a CAGR of **~26.4%**.

**Market Structure & Fragmentation**: The sector is **moderately fragmented**. Rather than being a single "winner-take-all" market, leadership is split across specialized domain niches:
- **Multiphysics & Engineering Simulation**: Dominant leaders include *Siemens* and *Ansys*.
- **AEC & Infrastructure Digital Twins**: Led by *Bentley Systems*.
- **High-Fidelity Rendering & Game Engines**: Led by *Epic Games (Unreal Engine)* and *Unity*.
- **3D Geospatial Data Streaming**: Led by *Cesium ion*.

---

## Commercial & Enterprise SaaS Platforms

| Product / Platform | Description & Key Strengths | Est. Company Valuation / Revenue | Starting Price / Paid Tiers | Free Tier / Free Trial Limits |
| :--- | :--- | :--- | :--- | :--- |
| **[AWS SimSpace Weaver](https://aws.amazon.com/simspaceweaver/)** | Managed spatial simulation service for millions of entities across cloud nodes. *(Ended support May 20, 2026; migrate to AWS Batch)*. | **$2.1 Trillion Market Cap** ($100B+ AWS Rev) | **$0.15 / SimUnit / hour** (or AWS Batch EC2 starting ~$0.0104/hr) | **AWS Free Tier**: 750 EC2 compute hours/mo + 60-day $300 cloud credit |
| **[Siemens Simcenter](https://plm.sw.siemens.com/)** | Predictive engineering multiphysics and system digital twin simulation platform. | **$150 Billion Market Cap** ($85B+ Annual Rev) | **$12,000 / year** per base 3D user license | **30-day Free Trial**: 10 free core-hours of Simcenter Cloud HPC |
| **[Ansys Twin Builder](https://www.ansys.com/)** | Multiphysics digital twin & system-level simulation environment for industrial assets. | **$35 Billion Valuation** ($2.3B Annual Rev) | **$15,000 / year** per concurrent user license | **Free Student Edition**: Unlimited time, restricted to 512,000 mesh nodes |
| **[Epic Games Unreal Engine Cloud](https://www.unrealengine.com/)** | Cloud pixel streaming & high-fidelity 3D rendering engine for spatial visualization. | **$31.5 Billion Valuation** ($5.8B Annual Rev) | **5% royalty** on gross revenue exceeding $1,000,000 per application | **Free Forever**: Full features free for projects under $1,000,000 gross revenue |
| **[Hexagon GeoMedia](https://www.hexagongeospatial.com/)** | Enterprise geospatial intelligence, GIS data management, and spatial analysis platform. | **$30 Billion Market Cap** ($5.8B Annual Rev) | **$3,500 / year** per desktop/enterprise license | **14-day Free Trial**: Full access via Hexagon Geospatial Portal |
| **[Bentley Systems iTwin](https://www.bentley.com/)** | Infrastructure digital twin platform for AEC, utilities, and smart urban modeling. | **$15 Billion Market Cap** ($1.2B Annual Rev) | **$500 / month** for iTwin Developer Commercial Plan | **Free Developer Plan**: 5 iTwin models, 1 GB storage, 1,000 API calls/month |
| **[Unity Simulation Pro](https://unity.com/)** | Distributed cloud-based simulation platform for robotics, autonomous vehicles, and synthetic data. | **$9 Billion Market Cap** ($2.1B Annual Rev) | **$2,040 / user / year** (Unity Pro) + **$0.05 / core-hour** | **Unity Personal Free**: Free for entities < $100k revenue; 14-day Pro trial |
| **[Cesium ion](https://cesium.com/platform/cesium-ion/)** | 3D geospatial data streaming platform for 3D Tiles, terrain, and high-scale globes. | **$15 Billion Parent Cap** (~$100M Standalone) | **$149 / month** (Commercial Tier, 100 GB storage / 500 GB streaming) | **Free Community Plan**: 5 GB storage, 50 GB/mo streaming, 1,000 uploads/mo |
| **[SimScale](https://www.simscale.com/)** | Browser-accessible cloud CFD, FEA, and thermal simulation software. | **$150 Million Valuation** ($15M Annual Rev) | **$600 / month** ($7,200/year billed annually for Professional Plan) | **Free Community Plan**: 3,000 core-hours/year (public project storage) |
| **[AnyLogic Cloud](https://www.anylogic.com/)** | Multimethod simulation engine (agent-based, discrete event, system dynamics) in the cloud. | **$80 Million Valuation** ($10M Annual Rev) | **$5,280 / year** per AnyLogic Professional license | **Free PLE (Personal Learning Edition)**: Free forever (up to 50,000 agents) |

---

## Top Open-Source Spatial Simulation Engines

Repos are listed in descending order by GitHub Star count.

### 1. [CesiumJS](https://github.com/CesiumGS/cesium) [![Stars](https://img.shields.io/github/stars/CesiumGS/cesium?style=social&color=white)](https://github.com/CesiumGS/cesium/stargazers)
- **License**: Apache-2.0
- **Category**: 3D Geospatial & Globe Visualization
- **Overview**: An open-source JavaScript library for world-class 3D globes and map visualization. Supports 3D Tiles and terrain streaming for large-scale spatial datasets.

### 2. [CARLA](https://github.com/carla-simulator/carla) [![Stars](https://img.shields.io/github/stars/carla-simulator/carla?style=social&color=white)](https://github.com/carla-simulator/carla/stargazers)
- **License**: MIT
- **Category**: Autonomous Driving Simulation
- **Overview**: Leading open-source autonomous driving simulator built on Unreal Engine. Features flexible sensor suites (LiDAR, RGB, Radar, GNSS), dynamic weather, NVIDIA PhysX vehicle dynamics, and ROS integration.

### 3. [Potree](https://github.com/potree/potree) [![Stars](https://img.shields.io/github/stars/potree/potree?style=social&color=white)](https://github.com/potree/potree/stargazers)
- **License**: BSD-2-Clause
- **Category**: Point Cloud & Geospatial Visualization
- **Overview**: WebGL-based point cloud renderer for massive spatial datasets. Built on Three.js, supporting fast web embedding and interactive measurement tools.

### 4. [Webots](https://github.com/cyberbotics/webots) [![Stars](https://img.shields.io/github/stars/cyberbotics/webots?style=social&color=white)](https://github.com/cyberbotics/webots/stargazers)
- **License**: Apache-2.0
- **Category**: Robotics & Agent Simulation
- **Overview**: Full-featured open-source robot simulator providing a complete development environment to model, program, and simulate autonomous vehicles and robotic agents.

### 5. [Eclipse SUMO](https://github.com/eclipse-sumo/sumo) [![Stars](https://img.shields.io/github/stars/eclipse-sumo/sumo?style=social&color=white)](https://github.com/eclipse-sumo/sumo/stargazers)
- **License**: EPL-2.0
- **Category**: Microscopic Urban Traffic Simulation
- **Overview**: Highly portable, microscopic traffic simulation package designed to model large city road networks, intermodal traffic (vehicles, pedestrians, public transit), and route optimization.

### 6. [Mesa](https://github.com/mesa/mesa) [![Stars](https://img.shields.io/github/stars/mesa/mesa?style=social&color=white)](https://github.com/mesa/mesa/stargazers)
- **License**: Apache-2.0
- **Category**: Agent-Based Modeling (ABM) Framework
- **Overview**: Open-source Python library for agent-based modeling of spatial, economic, and social systems. Features built-in spatial grids, agent scheduling, and Jupyter visualization.

### 7. [Project Chrono](https://github.com/projectchrono/chrono) [![Stars](https://img.shields.io/github/stars/projectchrono/chrono?style=social&color=white)](https://github.com/projectchrono/chrono/stargazers)
- **License**: BSD-3-Clause
- **Category**: Multibody Dynamics & Physics Engine
- **Overview**: High-performance C++ multi-physics simulation engine for ground vehicle dynamics, granular material flows, and large-scale mechanical systems.

### 8. [JSBSim](https://github.com/JSBSim-Team/jsbsim) [![Stars](https://img.shields.io/github/stars/JSBSim-Team/jsbsim?style=social&color=white)](https://github.com/JSBSim-Team/jsbsim/stargazers)
- **License**: LGPL-2.1
- **Category**: Flight Dynamics & Aerial Simulation
- **Overview**: Open-source Flight Dynamics Model (FDM) software library that models the flight mechanics of aircraft, rockets, and spacecraft.

### 9. [OpenFOAM](https://github.com/OpenFOAM/OpenFOAM-dev) [![Stars](https://img.shields.io/github/stars/OpenFOAM/OpenFOAM-dev?style=social&color=white)](https://github.com/OpenFOAM/OpenFOAM-dev/stargazers)
- **License**: GPL-3.0
- **Category**: Computational Fluid Dynamics (CFD)
- **Overview**: Premier open-source CFD solver framework offering customization for complex fluid dynamics, chemical reactions, heat transfer, and multiphysics modeling.

### 10. [Gazebo Sim](https://github.com/gazebosim/gz-sim) [![Stars](https://img.shields.io/github/stars/gazebosim/gz-sim?style=social&color=white)](https://github.com/gazebosim/gz-sim/stargazers)
- **License**: Apache-2.0
- **Category**: Robotics & ROS Simulation
- **Overview**: Next-generation Gazebo robotics simulator. Supports multiple physics engines (ODE, Bullet, DART, SimBody) and native integration with ROS / ROS 2.

### 11. [PDAL](https://github.com/PDAL/PDAL) [![Stars](https://img.shields.io/github/stars/PDAL/PDAL?style=social&color=white)](https://github.com/PDAL/PDAL/stargazers)
- **License**: BSD-3-Clause
- **Category**: Spatial Point Cloud Data Abstraction
- **Overview**: Point Data Abstraction Library (PDAL) — the spatial point cloud equivalent of GDAL for translating, filtering, and processing 3D LiDAR data.

### 12. [NetLogo](https://github.com/NetLogo/NetLogo) [![Stars](https://img.shields.io/github/stars/NetLogo/NetLogo?style=social&color=white)](https://github.com/NetLogo/NetLogo/stargazers)
- **License**: GPL-2.0
- **Category**: Agent-Based Spatial Environment
- **Overview**: Programmable modeling environment for simulating natural and social spatial phenomena, widely used in research and multi-agent systems modeling.

### 13. [FlightGear](https://github.com/FlightGear/flightgear) [![Stars](https://img.shields.io/github/stars/FlightGear/flightgear?style=social&color=white)](https://github.com/FlightGear/flightgear/stargazers)
- **License**: GPL-2.0
- **Category**: Flight & Atmospheric Simulator
- **Overview**: Advanced open-source flight simulator framework providing multi-display capability, PX4 flight controller integration, and world terrain rendering.

### 14. [AWSIM](https://github.com/autowarefoundation/AWSIM) [![Stars](https://img.shields.io/github/stars/autowarefoundation/AWSIM?style=social&color=white)](https://github.com/autowarefoundation/AWSIM/stargazers)
- **License**: Apache-2.0
- **Category**: Autoware Autonomous Driving Simulator
- **Overview**: Unity-based digital twin simulator created by TIER IV for Autoware autonomous driving integration with native ROS 2 message streaming.

### 15. [MATSim](https://github.com/matsim-org/matsim-libs) [![Stars](https://img.shields.io/github/stars/matsim-org/matsim-libs?style=social&color=white)](https://github.com/matsim-org/matsim-libs/stargazers)
- **License**: GPL-2.0
- **Category**: Agent-Based Transport Simulation
- **Overview**: Multi-Agent Transport Simulation framework designed for large-scale mobility, traffic demand, and public transit network modeling.

### 16. [OpenCourant](https://github.com/OpenCourant/OpenCourant) [![Stars](https://img.shields.io/github/stars/OpenCourant/OpenCourant?style=social&color=white)](https://github.com/OpenCourant/OpenCourant/stargazers)
- **License**: AGPL-3.0
- **Category**: Finite Element Analysis (FEA)
- **Overview**: Community fork of OpenRadioss for explicit finite element analysis (FEA), simulating dynamic impacts, structural crashes, and dynamic loading.

### 17. [City of Light (COL)](https://github.com/iliassarbout/CityOfLight) [![Stars](https://img.shields.io/github/stars/iliassarbout/CityOfLight?style=social&color=white)](https://github.com/iliassarbout/CityOfLight/stargazers)
- **License**: MIT
- **Category**: City-Scale Urban Embodied AI Simulator
- **Overview**: Unity-based digital twin of Paris (~116 km²) delivering high-throughput (~1300 FPS) multi-modal sensor streams (RGB, depth, normals, semantics) for AI research.

### 18. [MuPIF](https://github.com/mupif/mupif) [![Stars](https://img.shields.io/github/stars/mupif/mupif?style=social&color=white)](https://github.com/mupif/mupif/stargazers)
- **License**: LGPL-3.0
- **Category**: Distributed Multiphysics Workflows
- **Overview**: Modular, distributed integration platform for creating multi-scale multiphysics workflows and digital twin representations.

### 19. [VILLASnode](https://github.com/VILLASframework/villas-node) [![Stars](https://img.shields.io/github/stars/VILLASframework/villas-node?style=social&color=white)](https://github.com/VILLASframework/villas-node/stargazers)
- **License**: Apache-2.0
- **Category**: Real-Time Co-Simulation Gateway
- **Overview**: Real-time multi-protocol gateway enabling geographically distributed co-simulation across heterogeneous simulation models.

### 20. [Concordia Simulation Builder](https://github.com/ngstcf/concordia-sim-builder) [![Stars](https://img.shields.io/github/stars/ngstcf/concordia-sim-builder?style=social&color=white)](https://github.com/ngstcf/concordia-sim-builder/stargazers)
- **License**: Apache-2.0
- **Category**: Generative Agent Social Simulation
- **Overview**: No-code web interface for Google DeepMind's Concordia framework, enabling LLM-driven multi-agent social simulations.

---

## Framework Integration & Architecture Patterns

Building custom large-scale spatial simulation architectures typically requires hybrid composition:
- **Urban & Traffic Layer**: Combine **City of Light (COL)** or **Eclipse SUMO** for high-throughput traffic and city-scale multi-sensor observations.
- **Robotics & Vehicle Layer**: Deploy **CARLA** or **Gazebo** for hardware-in-the-loop and ROS 2 autonomous navigation benchmarking.
- **Generative Social Dynamics**: Utilize **Concordia Simulation Builder** or **Mesa** for LLM-based behavioral agent interaction.
- **Physics & Co-Simulation**: Interconnect solver engines using **MuPIF** or **VILLASframework** for distributed real-time multi-node execution.
- **3D Geospatial Visualization**: Stream spatial entity outputs using **CesiumJS** or **Potree** for browser-based 3D Tiles rendering.

---

## How to Contribute

Contributions are welcome! Please follow these simple guidelines:
1. Fork the repository.
2. Edit `README.md` maintaining clean Markdown tables and shields.io star badges.
3. Ensure entries include official documentation/repository links, factual descriptions, pricing/licensing details, and primary use cases.
4. Submit a Pull Request with a brief summary of additions or updates.

---

## Disclaimer & License Notes

- **Community Listing**: This list is community-curated for informational and research purposes.
- **Infrastructure Migration**: AWS SimSpace Weaver ended support on May 20, 2026. Users should migrate containerized workloads to AWS Batch.
- **Performance Trade-offs**: Open-source solvers (e.g. OpenFOAM) provide unmatched customization but require expert tuning to match commercial solver stability. High-fidelity rendering (CARLA, Unreal Engine) demands dedicated GPU hardware.
