# Filling Tank (Timers) - Factory IO PLC Project

**A clean, professional timer-based tank filling and discharging system** built in **Factory IO** with **IEC 61131-3 Ladder Logic**.


## 📋 Project Overview

**Project Name:** 3 - Filling Tank (Timers)  
**Objective:** Control the filling and emptying of a tank using **momentary push buttons** and **TON timers** only (no level sensors). Includes real-time countdown display on the control panel, safety interlocks, and clean cycle termination.

This is a classic Factory IO tutorial project that demonstrates core PLC programming skills: latching logic, timer control, HMI integration, and safety-first design.

**Status:** ✅ Fully functional and simulation-tested

## ✨ Key Features
- Independent **Fill** and **Discharge** cycles
- Momentary push-button latching with mutual exclusion (prevents both valves from opening at once)
- Precise TON timers: **43 seconds** (Fill) and **55 seconds** (Discharge)
- **Real-time countdown display** on the control panel (professional math block implementation)
- Automatic valve closure and display reset to 0 when the cycle ends
- Status outputs (`Filling` / `Discharging`) for HMI or panel lights
- Fail-safe design (valves close on PLC stop)

## 🛠️ Hardware & Software Used

| Component              | Details                                      |
|------------------------|----------------------------------------------|
| Simulator              | Factory IO v2.5.8 – Ultimate Edition        |
| PLC Software           | CODESYS (or any IEC 61131-3 compatible)     |
| Programming Language   | Ladder Logic (Structured)                    |
| Communication          | Factory IO driver (Modbus TCP / OPC UA)     |
| Inputs                 | Fill_PB, Discharge_PB (momentary)           |
| Outputs                | Fill_Valve, Discharge_Valve, Filling, Discharging, Timer_Display |


## 🚀 How to Run the Project

1. **Open Factory IO**
   - Load the scene: `Filling Tank (Timers)`
2. **Open your PLC project** in CODESYS (or compatible software)
3. **Import / Open** `PLC_PRG`
4. **Download** the program to the PLC
5. **Start simulation** in Factory IO
6. **Test**:
   - Press **Fill** button → tank fills, display counts down from 43
   - Press **Discharge** button → tank empties, display counts down from 55
   - Verify interlock (cannot start one cycle while the other is running)

## 📊 Skills Demonstrated (2026 PLC Portfolio)

- Professional latching logic with Set/Reset
- TON timer implementation and timing calculations
- Advanced math blocks (SUB, TO_INT, DIV, MOVE) for HMI integration
- Safety interlocks and fail-safe design
- Clean, maintainable, and well-documented code
- Full adherence to formal Requirements (R) specification

## 📄 Documentation

- [Full Requirements Specification](docs/Requirements-Spec.md)
- [Complete Ladder Logic PDF](docs/Filling-Tank-Code.pdf)

## 👤 Author

**Emmanuel E. Ajaegbu**  
PLC Programmer | Automation Engineer  
- X: [@iamajaegbu](https://x.com/iamajaegbu)  

## 📜 License

This project is open for educational and portfolio use. Feel free to use it as a reference.

**Made with ❤️ for the automation community**

