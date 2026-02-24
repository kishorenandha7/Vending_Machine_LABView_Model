🥤 Automated Sugarcane Juice Vending Machine (LabVIEW)
Project Overview
This repository contains a LabVIEW-based simulation of an automated sugarcane juice vending machine. Unlike standard snack dispensers, this project models a process-driven system that handles ingredient selection, crushing simulation, and real-time transaction logic.

The system is built using a State Machine Architecture, ensuring a modular and scalable design that mimics industrial control systems.

🛠 Features
Dynamic Pricing: Real-time calculation based on cup size and optional additives (e.g., Ginger, Lime, Ice).

State Machine Logic: Distinct states for Idle, Coin Insertion, Processing/Crushing, and Change Return.

Process Simulation: Includes a timed "Crushing" phase with progress indicators to simulate the mechanical extraction of juice.

Inventory Management: Tracks juice levels and waste (bagasse) capacity, triggering alerts when maintenance is required.

Safety Interlocks: Virtual sensors that prevent operation if the "Safety Door" is open or the "Waste Bin" is full.

🏗 System Architecture
The VI (Virtual Instrument) is organized into several key components:

Front Panel: An intuitive User Interface (UI) featuring numeric controls for payment, boolean switches for flavor selection, and a tank indicator to visualize the pouring process.

Block Diagram: * Main Control Loop: A While Loop containing a Case Structure (State Machine).

Data Persistence: Shift Registers are used to track the current balance, inventory, and machine status across iterations.

Event Handling: Uses an Event Structure for efficient user input processing.

🚀 How to Run
Clone the repository.

Open the .vi file in LabVIEW 2017 or later.

Click the Run arrow on the Front Panel.

Insert virtual currency, select your juice preferences, and click "Start" to begin the extraction process.
