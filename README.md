# Lego Mindstorms Pingpong Robot

This repository contains the implementation and design files for the **Lego Mindstorms Pingpong Robot**, developed as part of the **Lab 2: Pingpong Robot Competition**. The competition was organized under the **Intelligent Robotics Laboratory** course at **National Yang Ming Chiao Tung University (NYCU)**.

## Project Overview

The robot was designed with the following key features:
- **Efficient Ball Collection**: The robot uses a motor-driven mechanism to collect balls by pressing them against a wall.
- **Precise Ball Striking**: A motor-powered striking mechanism ensures accurate and fast delivery of balls to the opponent's field.
- **Symmetrical Design**: A rectangular and symmetric structure ensures stability and balance during movement.

The goal was to create a robot that could efficiently collect and return ping pong balls to the opponent's field while minimizing errors and time delays. This project combined mechanical design, programming, and sensor integration to achieve the desired functionality.

---

## Features

### 1. Robot Structure
- **Symmetrical and Rectangular Design**: The robot's frame is designed for stability and balance, preventing it from tilting during movement or ball collection.
- **Sensors**:
  - **Ultrasonic Sensor**: Measures the distance from walls to detect when the robot needs to turn.
  - **Light Sensor**: Detects if the robot enters the green zone to trigger the ball-striking mechanism.
  - **Motor Rotation Sensor**: Monitors motor angles to detect collisions and adjust movements.
- **Ball Striking Mechanism**: Composed of motor-connected cross axles that deliver quick and precise strikes.

### 2. Program Functionality
The robot's operations are divided into the following steps:
- **Wall Following and Collision Detection**:
  - The robot moves along a wall using a speed differential between the left and right motors to ensure smooth movement.
  - Rotation sensors monitor motor angles to detect collisions and trigger turning mechanisms.
- **Collision Recovery and Striking**:
  - Upon detecting a collision, the robot adjusts its position, moves to the striking location, and accelerates for 0.3 seconds to deliver the ball.
  - The light sensor ensures the robot strikes only within the designated area.
- **Post-Striking Reset**:
  - The robot retracts, resets its ball-collecting mechanism, and prepares for the next cycle.

---

## Files in This Repository

| File Name                             | Description                                                                 |
|---------------------------------------|-----------------------------------------------------------------------------|
| `Pingpong Robot.rbt`                  | Lego Mindstorms NXT program file controlling the robot's behavior.          |
| `lego-mindstorms-pingpong-robot_design.lxf` | Robot design file created with Lego Digital Designer.                         |
| `README.md`                           | Documentation describing the project and its implementation.                |

---

## How to Run

1. **Hardware Setup**:
   - Assemble the robot structure using the provided design file (`lego-mindstorms-pingpong-robot_design.lxf`) in Lego Digital Designer.
   - Upload the program file (`Pingpong Robot.rbt`) to the NXT robot using the Lego Mindstorms software.

2. **Software Execution**:
   - Place the robot at the starting position, oriented either left or right, depending on the parameter `Right` (`True` for right, `False` for left).
   - Start the program to initiate ball collection and striking.

3. **Results**:
   - The robot efficiently collects and returns balls to the opponent's field with minimal errors.

---

## Results and Achievements

- **Performance**:
  - Demonstrated consistent and stable performance during the competition.
  - Achieved first place in the final competition.
- **Video Demo**:
  - [Striking Mechanism Demo](https://youtube.com/shorts/Xh3lH8HGwqA)
  - [Final Competition](https://youtu.be/6f9M96ofsps)

---

## Learnings and Insights

- **Sensor Integration**:
  - Used rotation sensors to detect collisions and adjust robot movements dynamically.
- **Mechanical Design**:
  - Overcame challenges related to motor performance differences by fine-tuning speed settings for each motor.
- **Lego Digital Designer**:
  - Validated the robot's structure and design feasibility before assembly.
    <img src="https://github.com/user-attachments/assets/65779e12-9556-4861-9265-424882be1440" alt="Lego Digital Designer of Pingpong Robot" width="700"/>


---

## License

This project is released under the MIT License.

---

如果需要進一步修改或補充，請隨時告訴我！
