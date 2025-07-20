# Simverse

> A universal, modular, lightweight simulation engine designed to power robotics, drones, spacecraft, circuits, and quantum systems — from the core up.

## ✨ Key Features

- ⚙️ Modular Entity-Component System
- 🚀 Plugin-based physics (mechanical, electrical, quantum, digital)
- 🧩 Dynamic plugin loader for sensors, actuators, controllers
- 🧠 Real-time + headless simulation support
- 🖥️ Optional GUI via Bevy or Egui
- 📡 CLI & API control with data logging and replay
- ⚛️ Quantum and classical system simulation

## 🧱 Architecture

- `CoreSimEngine` – Fixed timestep manager & world scheduler
- `EntityManager` – Modular ECS for dynamic components
- `PhysicsCore` – Plugin-ready 2D/3D physics kernel
- `PluginSystem` – Load sensor/actuator/logic models
- `EventBus` – Component communication interface
- `Visualization` – Optional UI and sensor debug overlays

## 💡 What Can You Simulate?

- 🤖 Robot arms, wheeled bots
- 🛰️ Drones and autonomous spacecraft
- 🚗 Self-driving cars
- 🧮 Digital and analog circuits
- ⚛️ Quantum gates and entangled systems

## 🚀 Performance Benchmarks (MVP Target)

| Metric                  | Goal                              |
|-------------------------|-----------------------------------|
| Tick Rate (headless)    | 1000+ steps/sec                   |
| UI Startup              | <3s                               |
| Memory Footprint        | <10MB (core engine)               |
| Max Entities Supported  | 10,000                            |
| Plugin Load Time        | <50ms                             |

## 🛠 Tech Stack

- Language: **Rust**
- Physics: **Rapier**, optionally pluggable
- Visualization: **Bevy**, **Egui**
- Data: **Serde**, **SQLite**
- Future: ROS2, WebAssembly, AI agent integration

## 📦 Getting Started

```bash
git clone https://github.com/Paundra-Technologies/simverse
cd simverse
cargo run --example simple_robot
```

## 📍 Roadmap

-   Core engine + ECS
    
-   Mechanics + Physics plugins
    
-   Circuit simulation layer
    
-   Quantum module support
    
-   Visual UI / Replay tools
    
-   Web-based scenario designer
    

## 📄 License

MIT

## 🙌 Contribute

We welcome contributors! Check out the `CONTRIBUTING.md` and open an issue to get started.

----------

Built with ❤️ to simulate everything from bots to black holes.


[![](https://mermaid.ink/img/pako:eNp1VF1v4jAQ_CuWpd4T9PgIEcnDSdRE1DoClCSVeqYPvsQES4mNEvt0FPHfz0mAAlfe1jszu-vMOnsYy4RBF6YF3W5AOF4JAB4eAJIFA1Mpt9U5xOgnCXiuM6q4FJ_gO2i3fxjY90jIcwZ8KmjKiveTqIa9WYjDN-IJxdXua8pTFBDvDxMKPOkSfAdYKFasacwM7TjQYrMreVzWvatUU7VWL57fAowCcqJ4IuWC1R2OUE3zPfRMfBZvqKhYvkx09j8LRUE4908lkS6VzM_NF5k2pcvPqZDMt1JUgzflypvRAm8WzJckYKKUxWXLC84IhdEoNKxRrDRVd3ljPMHhaErGPOWKZsaAlMd3uAgvUYRD4mUsVgWPDR3xItZc3RG8RKNZGPnkRVOhdA4u3D4LjnfG8yowltXC6Xwy8ZZkTBWtJjpZe4JHC0zQFBtPTfSVr6-81DTjH02vb2DMfuv0ajlecUCuWRcGG7AmRZjUShOABRUsu9ic2jQzHE1YcVV5MY0meGYWp2EEu1KxvNmIBrnw8DZ7dOM2ffyOKwFb5knxBLqq0KwFc1bktDrCfSVZQbVhOVtB14QJW1OdqRVciYORban4JWV-UhZSpxvormlWmpPeJlSxMafmvebnbMGEuRuSWijoWk6vLgLdPfwL3Xbf6T46g8HAtjtW17J6ttWCO0OzHx270xl2nZ7TcfpO_9CCH3Xf7mNv2LEHjmU5w-7Q7naGLcgSbjbTb_4V9S_j8A9uVU_i?type=png)](https://mermaid.live/edit#pako:eNp1VF1v4jAQ_CuWpd4T9PgIEcnDSdRE1DoClCSVeqYPvsQES4mNEvt0FPHfz0mAAlfe1jszu-vMOnsYy4RBF6YF3W5AOF4JAB4eAJIFA1Mpt9U5xOgnCXiuM6q4FJ_gO2i3fxjY90jIcwZ8KmjKiveTqIa9WYjDN-IJxdXua8pTFBDvDxMKPOkSfAdYKFasacwM7TjQYrMreVzWvatUU7VWL57fAowCcqJ4IuWC1R2OUE3zPfRMfBZvqKhYvkx09j8LRUE4908lkS6VzM_NF5k2pcvPqZDMt1JUgzflypvRAm8WzJckYKKUxWXLC84IhdEoNKxRrDRVd3ljPMHhaErGPOWKZsaAlMd3uAgvUYRD4mUsVgWPDR3xItZc3RG8RKNZGPnkRVOhdA4u3D4LjnfG8yowltXC6Xwy8ZZkTBWtJjpZe4JHC0zQFBtPTfSVr6-81DTjH02vb2DMfuv0ajlecUCuWRcGG7AmRZjUShOABRUsu9ic2jQzHE1YcVV5MY0meGYWp2EEu1KxvNmIBrnw8DZ7dOM2ffyOKwFb5knxBLqq0KwFc1bktDrCfSVZQbVhOVtB14QJW1OdqRVciYORban4JWV-UhZSpxvormlWmpPeJlSxMafmvebnbMGEuRuSWijoWk6vLgLdPfwL3Xbf6T46g8HAtjtW17J6ttWCO0OzHx270xl2nZ7TcfpO_9CCH3Xf7mNv2LEHjmU5w-7Q7naGLcgSbjbTb_4V9S_j8A9uVU_i)
