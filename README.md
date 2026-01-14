# skeleton-proxy
A Mixed Reality framework that turns physical robots into immersive characters using VR Passthrough and local rendering.
# Skeleton Proxy: Hybrid Reality Robotics Framework

![Status](https://img.shields.io/badge/Status-Prototype-blueviolet)
![Platform](https://img.shields.io/badge/Platform-ROS2%20%7C%20Unity%20%7C%20UDP-lightgrey)
![License](https://img.shields.io/badge/License-MIT-green)

> "The Robot provides the Physical The VR provides the Soul."
>
> "Robot memberikan Fisika. VR memberikan Jiwa."

---

### 🌐 Language / Bahasa
[🇺🇸 **English Version**](#-english-version) | [🇮🇩 **Versi Bahasa Indonesia**](#-versi-bahasa-indonesia)

---

<a name="-english-version"></a>
## 🇺🇸 English Version

### 📡 The Vision
**Skeleton Proxy** is an open-source framework designed to solve the "Uncanny Valley" and "Lack of Touch" problems in modern robotics.

Instead of trying to build realistic silicone skin (which is expensive and static), we decouple the physical presence from the visual representation.
- The Hardware: An autonomous skeleton robot provides haptic feedback, warmth, and physical interaction.
- The Software: A VR Passthrough client renders high-fidelity characters (Anime, Furry, Humanoid) overlaid perfectly onto the skeleton.

### 🏗️ System Architecture
This repository is organized to enforce a clean separation of concerns between hardware, networking, and visualization.

```text
skeleton-proxy/
├── robot_core/       # ROS2 nodes & Motor control logic (The Body)
├── protocol/         # Low-latency UDP Telemetry Protocol (The Nervous System)
├── vr_client/        # Unity/Unreal Engine Client & IK Solvers (The Skin)
└── docs/             # Architecture diagrams & Setup guides
