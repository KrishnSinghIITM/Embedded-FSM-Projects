# ESP32 Traffic Light Controller

A simple and effective Finite State Machine (FSM) for controlling a traffic light, built for the ESP32.

## 🎥 Live Demo

* **See it live on Wokwi:** [Click here to run the simulation](https://wokwi.com/projects/438742735281832961)

* **Watch the video demo:** ![Traffic Light Simulation](https://github.com/KrishnSinghIITM/Embedded-FSM-Projects/blob/main/Project_01_TrafficLight/doc/demo.mp4?raw=true)


## 🚦 Features

* **Automatic Cycle:** The traffic light automatically cycles through Red, Green, and Yellow states using non-blocking timers.

* **Pedestrian Sensor:** A push button acts as a pedestrian sensor, allowing the Green light state to be interrupted for a faster cycle.

* **State-Based Logic:** Clean, readable, and efficient code built around a classic Finite State Machine pattern.

* **Wokwi Ready:** Includes a `diagram.json` for instant simulation.

## 📂 File Structure

* `README.md`: This documentation file.

* `src/`: Contains the main source code (`sketch.ino`) for the ESP32.

* `doc/`: Contains supporting documentation and diagrams, including the `diagram.json` for Wokwi.

## ⚙️ How It Works

The controller is built as a **Finite State Machine** with three states:

1. `STATE_RED`

2. `STATE_GREEN`

3. `STATE_YELLOW`

The system uses the `millis()` function to manage time without freezing the code with `delay()`. This allows the controller to be responsive to button presses at all times. The state transitions are triggered by either a timer expiring or a pedestrian request (button press) during the green light.

## 🛠️ Hardware

* ESP32 Development Board

* 1x Red LED

* 1x Yellow LED

* 1x Green LED

* 1x Push Button

* 3x 220Ω Resistors

* Breadboard and Jumper Wires
