# 🇩🇪 Hi, ich bin Daniel. 👋

Hauptberuflich arbeite ich als Projektleiter im Bereich ADAS. Meine eigentliche Leidenschaft ist jedoch die tiefgreifende, praktische Entwicklung. Um technologisch am Ball zu bleiben und komplexe Architekturen von Grund auf zu durchdringen, realisiere ich in meiner Freizeit anspruchsvolle Hardware- und Softwareprojekte.

Dabei bewege ich mich am liebsten an der Schnittstelle zwischen hardwarenaher Programmierung (Sensoren, PCBs, Mikrocontroller), algorithmischer Datenverarbeitung und der Anbindung an IoT-Infrastrukturen. In meinen Workflows setze ich zudem auf moderne, KI-gestützte Entwicklungsmethoden (AI-assisted Engineering), um Architekturen effizient und skalierbar auf den Code zu übertragen.

### 🛠️ Tech Stack & Hands-on Erfahrung
* **Software & Security:** C/C++, Python, Linux (IPC Tracing), ARM64 Assembly, Ghidra (Reverse Engineering)
* **Hardware & Algorithmen:** ESP32, DSP, KiCad (PCB Design), Sensor Fusion (EKF, IMM-CKF, AMCL Particle Filter, DBSCAN)
* **Architektur & Tools:** CI/CD (GitHub Actions), TDD, PlatformIO, LVGL, WebSockets, MQTT, CAN-Bus

---

### 🚀 Engineering-Projekte & Case Studies

#### 1. Smart Home Dashboard & Control Hub (C++ / PlatformIO)
[**Lela**](https://github.com/IamDiesel/Lela)
* **Was es ist:** Ein modulares Bedienpanel auf Basis eines ESP32-SoC, das UI, Echtzeit-Netzwerkkommunikation und dezentrale Hardware-Steuerung in einem Embedded-System vereint.
* **Highlights:** Native Integration von Home Assistant via WebSockets inklusive eines eigenen Lovelace-Dashboard-Parsers. Implementierung einer hochoptimierten Echtzeit-Video-Streaming-Pipeline, kombiniert mit pragmatischer Audio-Streaming-Logik. Umsetzung komplexer UI-Zustände mit der LVGL-Bibliothek und ereignisbasierter Steuerungen.

#### 2. Advanced Sensor Fusion & Tracking (M.Sc. Thesis / NVIDIA Jetson)
*(Code under NDA until 09/2026)*
* **Was es ist:** Entwicklung eines "Triple Radar & Camera"-Systems zur domänenübergreifenden Sensorfusion und zum Tracking von Fahrzeugen und Fußgängern.
* **Highlights:** Eigenständige Implementierung komplexer Algorithmen zur Objektverfolgung (**Extended Kalman Filter / EKF**) und zum Data-Clustering (**DBSCAN**). Lösung anspruchsvoller Datenassoziationsprobleme über Graph-basierte Ansätze (**GNN mit Auction Algorithm** für das gewichtete Zuordnungsproblem auf bipartiten Graphen) sowie mittels **KNN Cost Matrix** und dem **Jonker-Volgenant / Hungarian Algorithm**. Ausführung der gesamten Signalverarbeitungs-Pipeline auf einem Embedded NVIDIA Jetson System.

#### 3. System-Level Reverse Engineering (C++ / Linux)
[**DobbySpeak**](https://github.com/IamDiesel/D9DobbySpeak)
* **Was es ist:** Eine C++ Applikation zur Analyse und Modifikation des Laufzeitverhaltens eines kommerziellen Linux-basierten Robotersystems.
* **Highlights:** Blackbox-Analyse proprietärer Interprozesskommunikation (IPC) mittels System-Call-Tracing (`strace`). Entwicklung maßgeschneiderter C++ Parser, um die interne State Machine des Systems zu kapern und ereignisbasiert eigene Audio-Pipelines zu injizieren.

#### 4. Hardware Integration & IoT Middleware (Python / KiCad)
[**Alarm2Coffee**](https://github.com/IamDiesel/Alarm2Coffee)
* **Was es ist:** Eine physische Man-in-the-Middle-Hardwarelösung, um ein geschlossenes, konventionelles Haushaltsgerät vollständig in ein automatisiertes Ökosystem zu integrieren.
* **Highlights:** Vollständiges Schaltungs- und Platinendesign (KiCad PCB) zur Signalinterzeption auf Hardware-Ebene, gekoppelt mit einer ereignisgesteuerten Python-Middleware zur IoT-Anbindung via MQTT.

#### 5. Radar Data Engineering & DSP Modification (Embedded C / Python)
[**Dual Radar TI AWR1642**](https://github.com/IamDiesel/DUAL_RADAR_TI_AWR1642)
* **Was es ist:** Modifikation der Texas Instruments DSP-Firmware und Entwicklung einer Python-Datenpipeline als Fundament für ein IEEE-Forschungsprojekt.
* **Highlights:** Tiefer Eingriff in den C-Code des digitalen Signalprozessors zur erweiterten Rohdatenextraktion (Export der Doppler-Matrix) sowie hardwarenahes Bugfixing (Cosinus-Berechnung) und Rekonfiguration. Die extrahierten Daten wurden über eine maßgeschneiderte Python-Pipeline für das Training von Convolutional Neural Networks (CNNs).

#### 6. Mobile Security & ARM64 Reverse Engineering (Flutter/BoringSSL)
[**Kippy App Patcher**](https://github.com/IamDiesel/Android-RE-Patching-Framework/)
* **Was es ist:** Reverse Engineering einer proprietären Flutter-App zur Freilegung einer geschlossenen IoT-API, die als Basis für eine spätere Home Assistant Integration diente.
* **Highlights:** Statische Analyse und Modifikation von ARM64-Assembler-Code in einer statisch gelinkten BoringSSL-Bibliothek (Ghidra), um SSL-Pinning auf Betriebssystemebene auszuhebeln. Entwicklung eines eigenen Python-Frameworks (Tkinter) zur massiven Beschleunigung des iterativen Patch-, Signatur- und Flash-Zyklus inklusive automatisiertem Log-Parsing (Logcat).

#### 7. Enterprise-Grade API Integration & CI/CD (Python)
[**Kippy Home Assistant Integration**](https://github.com/IamDiesel/kippy-homeassistant-lola)
* **Was es ist:** Eine nach modernen Software-Engineering-Standards entwickelte Home Assistant Custom Component, basierend auf der zuvor per Reverse Engineering freigelegten API.
* **Highlights:** Stringente Umsetzung von Test-Driven Development (TDD) mit hoher Testabdeckung und modularer API-Kapselung. Aufbau vollständiger GitHub Actions CI/CD-Pipelines (HACS Validation, Flake8, Black) für kontinuierliche Code-Qualitätssicherung.

#### 8. Advanced BLE Tracking & Stochastics (Python)
[**TriLola / Bluecat Tracker**](https://github.com/IamDiesel/bluecat_26)
* **Was es ist:** Ein hochpräzises, stochastisches Indoor-Tracking-System (BLE/MQTT) zur Echtzeit-Lokalisierung über eine heterogene Sensorlandschaft (Unix, ESP32, Shelly).
* **Highlights:** Implementierung einer 5-stufigen Filterarchitektur, inklusive eines kinematischen AMCL-Partikelfilters und eines Interacting Multiple Model Constrained Kalman Filters (IMM-CKF). Dynamische Umgebungsmodellierung (SLAM/Tomographie) via Voxel-Grid zur Erkennung von Funkwiderständen und Hardware-Schwankungen im Mesh-Netzwerk.

---
📫 **Kontakt:** [LinkedIn](https://www.linkedin.com/in/daniel-kahrizi-745224215)

<br><br>

---

# 🇬🇧 Hi, I'm Daniel. 👋

Professionally, I work as a Technical Project Manager in the ADAS sector. However, my true passion lies in deep, hands-on engineering. To stay technologically sharp and thoroughly understand complex architectures from the ground up, I build advanced hardware and software projects in my free time.

My sweet spot is the intersection of low-level programming (sensors, PCBs, microcontrollers), algorithmic data processing, and IoT infrastructure integration. In my workflows, I heavily leverage modern, AI-assisted engineering methods to translate architectures into scalable code efficiently.

### 🛠️ Tech Stack & Hands-on Experience
* **Software & Security:** C/C++, Python, Linux (IPC Tracing), ARM64 Assembly, Ghidra (Reverse Engineering)
* **Hardware & Algorithms:** ESP32, DSP, KiCad (PCB Design), Sensor Fusion (EKF, IMM-CKF, AMCL Particle Filter, DBSCAN)
* **Architecture & Tools:** CI/CD (GitHub Actions), TDD, PlatformIO, LVGL, WebSockets, MQTT, CAN-Bus

---

### 🚀 Engineering Projects & Case Studies

#### 1. Smart Home Dashboard & Control Hub (C++ / PlatformIO)
[**Lela**](https://github.com/IamDiesel/Lela)
* **What it is:** A modular control panel based on an ESP32 SoC that unifies UI, real-time network communication, and decentralized hardware control in one embedded system.
* **Highlights:** Native Home Assistant integration via WebSockets, including a custom Lovelace dashboard parser. Implemented a highly optimized real-time video streaming pipeline combined with pragmatic audio streaming logic. Realized complex UI states using the LVGL library and event-driven controls.

#### 2. Advanced Sensor Fusion & Tracking (M.Sc. Thesis / NVIDIA Jetson)
*(Code under NDA until 09/2026)*
* **What it is:** Development of a "Triple Radar & Camera" system for cross-domain sensor fusion and tracking of vehicles and pedestrians.
* **Highlights:** Independent implementation of complex tracking algorithms (**Extended Kalman Filter / EKF**) and data clustering (**DBSCAN**). Solved challenging data association problems using graph-based approaches (**GNN with Auction Algorithm** for weighted bipartite matching) as well as **KNN Cost Matrices** and the **Jonker-Volgenant / Hungarian Algorithm**. Deployed the entire signal processing pipeline on an embedded NVIDIA Jetson system.

#### 3. System-Level Reverse Engineering (C++ / Linux)
[**DobbySpeak**](https://github.com/IamDiesel/D9DobbySpeak)
* **What it is:** A C++ application for analyzing and modifying the runtime behavior of a commercial Linux-based robot system.
* **Highlights:** Blackbox analysis of proprietary Inter-Process Communication (IPC) using system call tracing (`strace`). Developed custom C++ parsers to hijack the system's internal state machine and inject custom event-driven audio pipelines.

#### 4. Hardware Integration & IoT Middleware (Python / KiCad)
[**Alarm2Coffee**](https://github.com/IamDiesel/Alarm2Coffee)
* **What it is:** A physical man-in-the-middle hardware solution to fully integrate a closed, conventional household appliance into an automated ecosystem.
* **Highlights:** End-to-end circuit and PCB design (KiCad) for hardware-level signal interception, coupled with event-driven Python middleware for IoT connectivity via MQTT.

#### 5. Radar Data Engineering & DSP Modification (Embedded C / Python)
[**Dual Radar TI AWR1642**](https://github.com/IamDiesel/DUAL_RADAR_TI_AWR1642)
* **What it is:** Modification of Texas Instruments DSP firmware and development of a Python data pipeline as the foundation for an IEEE research project.
* **Highlights:** Deep modification of the digital signal processor's C code for advanced raw data extraction (Doppler matrix export), alongside hardware-level bug fixing (cosine calculation) and reconfiguration. The extracted data was processed via a custom Python pipeline to train Convolutional Neural Networks (CNNs).

#### 6. Mobile Security & ARM64 Reverse Engineering (Flutter/BoringSSL)
[**Kippy App Patcher**](https://github.com/IamDiesel/Android-RE-Patching-Framework/)
* **What it is:** Reverse engineering of a proprietary Flutter app to expose a closed IoT API, serving as the basis for a subsequent Home Assistant integration.
* **Highlights:** Static analysis and modification of ARM64 assembly within a statically linked BoringSSL library (Ghidra) to bypass OS-level SSL pinning. Developed a custom Python framework (Tkinter) to massively accelerate the iterative patch, sign, and flash cycle, including automated log parsing (Logcat).

#### 7. Enterprise-Grade API Integration & CI/CD (Python)
[**Kippy Home Assistant Integration**](https://github.com/IamDiesel/kippy-homeassistant-lola)
* **What it is:** A Home Assistant custom component developed to modern software engineering standards, utilizing the API exposed via reverse engineering.
* **Highlights:** Strict implementation of Test-Driven Development (TDD) with high test coverage and modular API encapsulation. Setup of full GitHub Actions CI/CD pipelines (HACS Validation, Flake8, Black) for continuous code quality assurance.

#### 8. Advanced BLE Tracking & Stochastics (Python)
[**TriLola / Bluecat Tracker**](https://github.com/IamDiesel/bluecat_26)
* **What it is:** A highly precise, stochastic indoor tracking system (BLE/MQTT) for real-time localization across a heterogeneous sensor landscape (Unix, ESP32, Shelly).
* **Highlights:** Implemented a 5-stage filter architecture, including a kinematic AMCL Particle Filter and an Interacting Multiple Model Constrained Kalman Filter (IMM-CKF). Dynamic environment modeling (SLAM/Tomography) via a voxel grid to detect radio resistance and hardware fluctuations in the mesh network.

---
📫 **Get in touch:** [LinkedIn](https://www.linkedin.com/in/daniel-kahrizi-745224215)
