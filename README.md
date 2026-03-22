# Brick Breaker Game

This project is a **brick breaker game** developed using **Arduino and an OLED display**. The game features a **paddle controlled by a potentiometer**, a **moving ball**, and **breakable brick layouts**. An **LDR sensor adds a screen inversion effect based on ambient light**. In addition, the game becomes progressively more difficult and includes a **life system**.

---

## Features

- **Paddle control using a potentiometer**
- **Automatically moving ball mechanic**
- **Different brick layouts across levels**
- **Ambient light detection with an LDR sensor and screen inversion effect**
- **Increasing ball speed as levels progress**
- **Life gain mechanic with heart objects**
- **Score display using a Seven Segment Display**

---

## Hardware Requirements

You will need the following components to build this project:

- **Arduino (Uno, Mega, etc.)**
- **128x64 OLED display (SSD1306)**
- **Potentiometer**
- **LDR (Light Sensor)**
- **3 LEDs** (for life status visualization)
- **3 Buttons (Up, Down, Select)**
- **7 Segment Display**
- **Jumper wires**

---

## Installation and Usage

### 1. Clone the Repository

Run the following command in your terminal or command prompt:

```sh
git clone https://github.com/Esentrn/Brick-Breaker-Game.git
cd Brick-Breaker-Game
```

### 2. Connections

Below are the **connections between the Arduino and the components**:

- **OLED Display**
  - VCC → 5V
  - GND → GND
  - SDA → A4 (for Arduino Uno)
  - SCL → A5 (for Arduino Uno)

- **LDR Sensor** → A2
- **Potentiometer** → A0

- **LED Connections**
  - LED1 → 8
  - LED2 → 9
  - LED3 → 13

- **Buttons**
  - Up → 12
  - Down → 11
  - Select → 10

- **7 Segment Display**
  - Segment A → 1
  - Segment B → 2
  - Segment C → 3
  - Segment D → 4
  - Segment E → 5
  - Segment F → 6
  - Segment G → 7

### 3. Uploading the Code

You can upload the project using **Arduino IDE** or **PlatformIO** by following these steps:

1. **Install the required libraries:**
   - `Adafruit_GFX`
   - `Adafruit_SSD1306`
2. **Upload the code to the Arduino.**
3. **Check the connections and connect the Arduino.**
4. **Select the correct board and port in the Arduino IDE.**
5. **Compile and upload the code.**

---

## Game Mechanics

### Starting the Game

- The menu includes the options **"1. Start"** and **"2. Exit"**.
- When **Start** is selected, the ball begins to move.

### Paddle Control

- The paddle is moved left and right using the potentiometer.

### Ball Movement

- The ball bounces back when it hits the screen boundaries.
- When it hits brick layouts, the bricks break and the score increases.

### Levels and Score

- There are **5 different brick layouts** in total.
- The brick arrangement changes at each level.
- If all bricks are broken, the game **moves to the next level** and the ball speed increases.

### Life System and Hearts

- The player starts with **3 lives**.
- **LEDs display the current life status**.
- **Heart objects randomly fall**, and if caught, the player gains **an extra life**.
- If all lives are lost, the game ends.

### Game Over

- If all lives are depleted, the game ends and the **score is displayed on the screen**.
- The message **"Game Over!"** is shown, and the game returns to the menu.

---

## Visual

![Game Screen](https://github.com/Esentrn/Brick-Breaker-Game/blob/01c15635e28c1c352f8bf83abcd27e9a3439a8f3/Brick-Breaker-Game.png)

---

## Game Video

![Game Preview](https://github.com/Esentrn/Brick-Breaker-Game/blob/01c15635e28c1c352f8bf83abcd27e9a3439a8f3/Brick-Breaker-Game.gif)

---

Enjoy the game! 🎉
