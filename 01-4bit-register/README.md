# 📦 4-Bit Parallel Storage Register (PIPO)
A synchronous **4-Bit Parallel-In Parallel-Out (PIPO) Register** simulated in **Proteus Design Suite**. Constructed using discrete D Flip-Flops (`DTFF`), this circuit stores a 4-bit binary input simultaneously on a clock pulse.
---
## 📌 Key Features
* **Architecture:** Parallel-In / Parallel-Out (PIPO).
* **Synchronous Operation:** All flip-flops share a single clock line for simultaneous data latching.
* **Storage Capacity:** 4 Bits ($D_0, D_1, D_2, D_3$).
* **Output Display:** Real-time visual monitoring via Pink LEDs (`D1`–`D4`).
---
## 📐 Circuit Schematic & Simulation
### 1. Circuit Schematic

<img width="1920" height="1080" alt="Screenshot (91)" src="https://github.com/user-attachments/assets/7d1a9fc2-98f6-4e0b-9824-4bd1a9a3e1e9" />



### 2. Live Simulation



https://github.com/user-attachments/assets/18376df5-f624-4bac-a05e-727847cfd1b5


---
## 🧠 Working Principle
1. **Data Setting:** Binary states (`0` or `1`) are selected using interactive LOGICSTATE switches connected to the $D$ inputs of flip-flops `U1` through `U4`.
2. **Data Latching:** On the active edge of the shared clock signal, the logic levels present on the $D$ inputs are captured into memory simultaneously.
3. **Data Retention:** Outputs ($Q_0$–$Q_3$) maintain their saved state independently of input switches until the next active clock transition, illuminating the Pink LEDs (`D1`–`D4`).
---
## 🛠️ Hardware Components Simulated

| Component | Model / Identifier | Function / Description |
| :--- | :--- | :--- |
| **EDA Tool** | Proteus 9 Professional | Simulation Environment |
| **Flip-Flops** | **DTFF** (`U1`–`U4`) | 1-Bit Data Storage Elements |
| **Inputs** | **LOGICSTATE** Switches | 4-Bit Data Input ($D_0$–$D_3$) |
| **Outputs** | **LED-PINK** (`D1`–`D4`) | Logic State Output Indicators |
| **Clock Source** | Digital Clock Generator | Shared Synchronous Clock Input |

---
## 💾 How to Run
1. Open [`register_4bit.pdsprj`](./4bit-register.pdspri) in **Proteus 9** or higher.
2. Set input values via logic switches and observe how outputs update synchronously with the clock signal.
