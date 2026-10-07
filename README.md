# Awesome-Large-Scale-Spatial-Simulation

## Top Large-Scale Spatial Simulation Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on City-Scale Simulation, Digital Twins & Self-Hosted Spatial Engines*

**Last updated: October 2026**



This repository tracks notable **commercial large-scale spatial simulation platforms** and **open-source projects** that simulate millions of interacting entities across geographic space — powering urban planning, autonomous vehicle testing, disaster evacuation modeling, and digital twin research.



**Examples** include AWS SimSpace Weaver, Bentley Systems iTwin, Cesium ion, Epic Games Unreal Engine Cloud, Unity Simulation Pro, Ansys Twin Builder, SimScale, AnyLogic Cloud, Siemens Simcenter, and Hexagon GeoMedia (the category leaders).



**Open-source emphasis**: Large-scale spatial simulation is anchored by **Gazebo** and **CARLA** for robotics and autonomous vehicle testing, **City of Light (COL)** for city-scale urban simulation, **Concordia Simulation Builder** for generative agent-based social simulation, **OpenFOAM** for multiphysics simulation, **MuPIF** for distributed multiphysics workflows, **VILLASframework** for real-time co-simulation, and **OpenCourant** as the community fork of OpenRadioss for finite element analysis. **Potree** and **CesiumJS** handle point cloud and geospatial visualization. This section is heavily expanded.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[AWS SimSpace Weaver](https://aws.amazon.com/simspaceweaver/)**

  **AWS's managed spatial simulation service** — distributed millions of entities across multiple servers for city-scale crowd simulation, traffic flow, and evacuation modeling . **Automatic spatial partitioning** splits simulation space into grid cells assigned to worker nodes, with transparent cross-boundary entity interaction handling . **Unreal Engine and Unity integration** for real-time 3D visualization with LOD control for rendering millions of entities . **Note**: Service **ended support May 20, 2026** — AWS recommends migrating containerized simulations to AWS Batch .



- **[Bentley Systems iTwin](https://www.bentley.com/)**

  **Infrastructure digital twin platform** — synchronized physical and digital infrastructure for AEC and utilities. **iTwin.js is available as open-source** and was identified as the best open-source option for net-zero manufacturing applications . **Best for infrastructure digital twins**.



- **[Cesium ion](https://cesium.com/platform/cesium-ion/)**

  **3D geospatial data streaming platform** — hosts and streams 3D Tiles, terrain, and imagery for large-scale geospatial visualization. **CesiumJS is open-source** for the viewer component, though storing and serving terrain to the viewer requires a paid subscription . **Best for geospatial visualization at scale**.



- **[Epic Games Unreal Engine Cloud](https://www.unrealengine.com/)**

  **Cloud deployment for Unreal Engine** — pixel streaming and cloud rendering for large-scale simulation visualization. **Unreal Engine is open-source** for the engine itself, with cloud services for deployment . **Best for high-fidelity simulation rendering**.



- **[Unity Simulation Pro](https://unity.com/)**

  **Cloud-based simulation at scale** — distributed simulation execution for robotics and autonomous systems. **Unity is not open-source** but well-documented with reasonable customizability when combined with open-source code . **Best for Unity-based simulation workflows**.



- **[Ansys Twin Builder](https://www.ansys.com/)**

  **Multiphysics digital twin platform** — build, validate, and deploy digital twins for complex systems . **Best for engineering digital twins**.



- **[SimScale](https://www.simscale.com/)**

  **Cloud-based simulation platform** — browser-accessible CFD and FEA with scalable computing resources . **Best for accessible cloud simulation**.



- **[AnyLogic Cloud](https://www.anylogic.com/)**

  **Multimethod simulation platform** — agent-based, discrete event, and system dynamics simulation in the cloud. **Best for business and social simulation**.



- **[Siemens Simcenter](https://plm.sw.siemens.com/)**

  **Simulation and test solutions** — integrated multiphysics simulation for product development. **Note**: Siemens acquired Altair and integrated Radioss into Simcenter, discontinuing the OpenRadioss open-source project . **Best for enterprise engineering simulation**.



- **[Hexagon GeoMedia](https://www.hexagongeospatial.com/)**

  **Geospatial intelligence platform** — GIS analysis and spatial data management . **Best for geospatial analysis workflows**.



## Open-Source GitHub Projects



### City-Scale Urban Simulation



- **[City of Light (COL)](https://github.com/iliassarbout/CityOfLight)**

  **City-scale, geo-anchored urban simulator for high-throughput embodied AI research**, open-source . **Covers ~116 km² of inner Paris** built from public GIS sources (OpenStreetMap, IGN, Paris Data) with per-tile meshes . **Four synchronized sensor modalities per frame**: RGB, depth, normals, and semantics . **TURBO Unity-Python bridge** streams multi-camera observations at up to **~1300 FPS** (RTX 4090), achieving higher throughput than ML-Agents . **Stochastic traffic and pedestrian flows** with configurable scenarios . **Street View Digital Twin** aligns simulator viewpoints with real-world panoramas for frame-accurate comparison . **Best for urban embodied AI and reinforcement learning research**.



- **[Gazebo](https://github.com/gazebosim/gz-sim)**

  **Open-source robotics simulator from Open Source Robotics Foundation**, Apache-2.0 licensed . **Default simulator in Robot Operating System (ROS)** with active community . **Supports multiple physics engines**: ODE, Bullet, SimBody, DART . **Modular architecture** with separate libraries for physics, rendering, UI, communication, and sensor generation . **UAV support includes quadrotors (Iris, Solo), hexarotors (Typhoon H480), and VTOL aircraft** . **Arena-Rosnav-3D** extends Gazebo with realistic dynamic 3D scenarios for ROS navigation benchmarking . **Best for robotics simulation and ROS integration**.



### Generative Agent-Based Simulation



- **[Concordia Simulation Builder](https://github.com/ngstcf/concordia-sim-builder)**

  **No-code web interface for Google DeepMind's Concordia framework**, Apache-2.0 licensed . **38 ready-to-run templates** covering SDG research, game theory, cybersecurity, and policy analysis . **9-tab analytics dashboard** with batch runs, parameter sweeps, and CSV/JSON export . **8 LLM providers supported**: OpenAI, Azure OpenAI, Anthropic, Gemini, DeepSeek, GLM, and Ollama (local or remote) . **Automatic checkpoints with resume-and-extend workflow** . **Democratizes AI social simulation** by making generative agent-based modeling accessible without coding . **Best for social simulation and LLM-driven agent research**.



### Autonomous Vehicle & Robotics Simulation



- **[CARLA](https://github.com/carla-simulator/carla)**

  **The leading open-source autonomous driving simulator**, MIT licensed with **14,000+ GitHub stars** . **Unreal Engine-based with realistic urban environments** . **Configurable sensor suites (LiDAR, cameras, radar, GNSS, IMU)** . **Vehicle dynamics based on NVIDIA PhysX engine** . **Python/C++ APIs with ROS bridge** . **Scenario runner for reproducible testing** . **Best for autonomous driving RL research**.



- **[AWSIM](https://github.com/tier4/AWSIM)**

  **Unity-based autonomous driving simulator from TIER IV**, Apache-2.0 licensed . **Designed as reference environment for Autoware** . **Native ROS 2 interface available** . **Trade-offs**: limited scenario library, no scaling features, smaller community . **Best for Autoware-native simulation**.



### Multiphysics & Digital Twin Simulation



- **[MuPIF](https://github.com/mupif/mupif)**

  **Open-source, modular, object-oriented simulation platform for distributed multiphysics workflows**, LGPLv3 licensed . **Data Management System (DMS)** builds digital twin representations with full traceability . **Graphical Workflow Editor** for low-code workflow development . **Standardizes application and data component interfaces** for seamless integration of different simulation models . **HPC integration** for high computational needs . **SSL or VPN-based secure communication** . **Best for complex multiphysics digital twins**.



- **[OpenFOAM](https://github.com/OpenFOAM/OpenFOAM-dev)**

  **Open-source CFD framework with unrivaled customization potential**, GPL-3.0 licensed . **No direct software cost** but requires investment in skilled personnel . **Requires expert-tuned settings** to achieve stability comparable to commercial solvers . **Best for research teams implementing novel models**.



- **[OpenCourant](https://github.com/OpenCourant/OpenCourant)**

  **Community fork of OpenRadioss for finite element analysis**, GNU AGPLv3 licensed . **Continues the OpenRadioss project after Siemens discontinued it** following the Altair acquisition . **Created by Brian Clemens, founder of RESF (Rocky Enterprise Software Foundation)** . **Best for FEM simulation with open governance**.



### Real-Time Co-Simulation



- **[VILLASframework](https://github.com/VILLASframework)**

  **Toolset for local and geographically distributed real-time co-simulation** . **Key components**: **VILLASnode** — open-source real-time multi-protocol gateway (C++, 15 stars) . **VILLASweb** — frontend for planning, controlling, monitoring, and analyzing distributed simulations (JavaScript, 3 stars) . **VILLAScontroller** — control and monitor simulation resources via AMQP/RabbitMQ (Python) . **VILLASsignaling** — WebSocket server for WebRTC signaling . **Best for distributed co-simulation workflows**.



### Geospatial Visualization



- **[Potree](https://github.com/potree/potree)**

  **WebGL-based point cloud viewer for large datasets**, open-source . **Outperformed CesiumJS in weighted comparison** for point cloud visualization: higher scores for documentation, UI, out-of-the-box options, and ease of embedding . **Built on Three.js, CesiumJS, and D3.js** . **Simple to embed in websites** with iframe support . **Best for point cloud visualization**.



- **[CesiumJS](https://github.com/CesiumGS/cesium)**

  **Open-source JavaScript library for 3D geospatial visualization**, Apache-2.0 licensed . **3D Tiles and terrain streaming** — Cesium ion required for hosting terrain . **Strong documentation and measurement tools** . **Widely used for geospatial applications** . **Trade-off**: terrain hosting requires paid subscription . **Best for geospatial visualization on a globe**.



### Additional Strong Open-Source Options



- **Ignition (now Gazebo)** — Next-generation Gazebo with DART physics engine .

- **Webots** — Open-source robot simulator with ROS 2 support .

- **FlightGear** — Advanced open-source flight simulator with PX4 support .

- **JSBSim** — Open-source flight dynamics model for aircraft and rockets .

- **Open Simulation Platform (OSP)** — Maritime industry simulation platform from DNV GL, NTNU, Rolls-Royce, and SINTEF Ocean .



**Frameworks for building custom large-scale spatial simulation solutions**: Combine **City of Light (COL)** for city-scale urban simulation with high-throughput multi-sensor streams . Use **Gazebo** for robotics simulation with ROS integration and multiple physics engines . Deploy **Concordia Simulation Builder** for generative agent-based social simulation with LLM providers . Choose **MuPIF** for distributed multiphysics digital twins with workflow editor . Integrate **VILLASframework** for real-time co-simulation across distributed resources . Use **Potree** or **CesiumJS** for geospatial visualization . Note that true enterprise large-scale spatial simulation with managed infrastructure, global scale, and vendor-supported SLAs (Bentley iTwin, Cesium ion, Ansys Twin Builder) remains primarily commercial territory; open-source stacks provide strong urban simulation, robotics testing, and multiphysics foundations that require integration for complete spatial simulation platforms.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Large-scale spatial simulation platforms handle computationally intensive workloads and may process sensitive geospatial data. Self-hosted solutions require proper security hardening, access controls, and compliance with data privacy regulations.

- **AWS SimSpace Weaver ended support May 20, 2026** — migrate containerized simulations to AWS Batch for execution infrastructure .

- **Gazebo rendering is less advanced than Unreal Engine or Unity** — suitable for robotics testing but not high-fidelity visualization . **CARLA and COL provide higher-fidelity visuals** at higher computational cost.

- **Commercial solvers converge faster than open-source alternatives** — OpenFOAM requires expert tuning to achieve comparable stability, though it offers unrivaled customization .

- **License considerations**: Gazebo uses Apache-2.0 , CARLA uses MIT , Concordia Simulation Builder uses Apache-2.0 , MuPIF uses LGPLv3 , OpenFOAM uses GPL-3.0 , and OpenCourant uses GNU AGPLv3 . Verify licensing against your use case before committing.

- The open-source ecosystem provides strong urban simulation, robotics testing, and multiphysics foundations, but **managed infrastructure, global scale, and vendor-supported SLAs** remain primarily commercial offerings.
