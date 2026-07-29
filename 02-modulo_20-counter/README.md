# 🔢 Modulo-20 Synchronous/Ripple Counter (0 to 19)
A sequential digital logic circuit designed and simulated in **Proteus Design Suite**. Constructed directly from discrete **CD4013 D Flip-Flops**, this counter counts sequentially from `0` to `19`
and automatically resets back to `0` upon reaching state `20` ($10100_2$).
---
## 📌 Features & Highlights
* **Counting Sequence:** Modulo-20 (`00` to `19` Decimal).
* **Architecture:** Built from scratch using discrete **CD4013 D-Type Flip-Flops** instead of integrated counter ICs.
* **Combinational Reset Logic:** Uses **AND gates** and a **NOT gate** to decode state `20` ($10100_2$) and feed an immediate reset pulse.
* **Real-time Monitoring:** Features **Logic Probes** for line status debugging and a **BCD 7-Segment Display** for numerical visual output.
---
## 📐 Circuit Schematic



<img width="1920" height="1080" alt="Screenshot (92)" src="https://github.com/user-attachments/assets/174488c1-59f3-41fe-bf70-7009e3973316" />

---
## 🎬 Live Simulation Demo

https://github.com/user-attachments/assets/c9fd7c63-3a0b-4bac-be35-92122ab56499
 
---
## 🧠 Circuit Working Principle
1. **Clock Input:** A pulse generator (`CLOCK`) drives the system logic.
2. **Cascaded Flip-Flops:** The **4013 D Flip-Flops** (`U8`, `U10`, `U1`) are configured to handle the sequential binary count.
3. **State Decoding:** The **AND** gates (`U2`, `U5`) combined with the **NOT** gate (`U3`) continuously monitor the bit outputs to detect binary state `20` ($10100_2$).
4. **Asynchronous Reset:** Upon reaching state 20, a `HIGH` signal is triggered and fed directly into the `RESET` pins of the flip-flops, instantly clearing the counter back to `00`.
---
## 🛠️ Hardware Components Simulated

| Component Name (Proteus) | Type / Library | Function in Circuit |
| :--- | :--- | :--- |
| **`4013`** | Dual D-Type Flip-Flop | Discrete Counter Stages (`U8`, `U10`, `U1`) |
| **`AND`** | Logic Gate | Binary State Decoding (`U2`, `U5`) |
| **`NOT`** | Logic Gate | Logic Inversion for Reset Decoding (`U3`) |
| **`7SEG-BCD`** | BCD 7-Segment Display | Direct Numerical Output Display |
| **`LOGICPROBE (BIG)`** | Visual Logic State Indicator | Real-time Signal State Debugging (`?`) |
| **`CLOCK`** | Digital Clock Generator | Pulse Clock Source |

---
## 💾 How to Run
1. Open `counter_m20.pdsprj` in **Proteus 9** or higher.
2. Press the **Play** button at the bottom left to start counting from 0 to 19.
