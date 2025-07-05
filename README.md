# 🎛️ PID Controller Simulation using Op-Amps | LTSpice / Proteus

A simulated **analog PID (Proportional-Integral-Derivative) controller** implemented using operational amplifiers to control a DC motor's speed. This project demonstrates how PID control theory can be physically modeled using analog electronics rather than digital microcontrollers.

## 🎯 Objective
To simulate a standalone analog PID control loop capable of minimizing error between a reference input and a system's output, such as a motor’s speed or position.

## ⚙️ Technologies & Tools Used
| Domain                | Tools/Components                     |
|-----------------------|--------------------------------------|
| Circuit Simulation    | LTSpice, Proteus, Multisim           |
| Core Components       | LM741 / TL081 Op-Amps                |
| Supporting Components | Resistors, Capacitors, DC motor model|
| Power Supply          | ±12V Dual Power Supply               |

## 🛠️ System Overview
- **Proportional Section:** Non-inverting amplifier with gain set by resistor ratio.
- **Integral Section:** Inverting integrator using op-amp, resistor, and capacitor.
- **Derivative Section:** Inverting differentiator circuit with resistor-capacitor network.
- The three stages are combined to form the complete PID control block.
- The controller receives an **error signal (reference - feedback)** and adjusts the motor's input voltage accordingly.

## 🧪 Simulation Process
- Model the motor as a first-order lag system or use a predefined DC motor block.
- Inject a step or sinusoidal reference signal.
- Observe the reduction in steady-state error (P), overshoot control (D), and offset correction (I).
- Fine-tune resistor and capacitor values to optimize performance.

## ✅ Key Features
- Fully analog PID response with no microcontroller.
- Real-time continuous control without sampling delays.
- Easily tunable P, I, and D gains via resistor-capacitor adjustment.
- Demonstrates classical control system design in a hardware-representative environment.

## 🔧 Future Improvements
- Convert the analog design into a mixed-signal system (analog PID, digital motor feedback).
- Replace with precision op-amps for improved accuracy.
- Fabricate a PCB for real-world PID motor control applications.

