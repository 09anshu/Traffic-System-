# Adaptive Traffic Light Management System

## Overview
This project simulates an Adaptive Traffic Light Management System using HTML, CSS, and JavaScript. It features a graphical intersection where cars and ambulances interact with traffic lights that adjust their cycle times based on traffic load. The simulation includes realistic road elements, dynamic vehicle creation, and real-time traffic metrics.

## Features
- **Dynamic Intersection Visualization**: A 2D graphical simulation of an intersection with vertical and horizontal roads, traffic lights, and bypass lanes.
- **Traffic Lights with Adaptive Timing**: Traffic lights adapt their cycle times to manage vehicle flow, changing between `North-South` and `East-West` phases based on traffic conditions.
- **Vehicle Simulation**: Cars and ambulances appear at random intervals, move across the intersection, and respect traffic lights.
- **Ambulance Priority**: Ambulances bypass waiting traffic and move through the intersection, simulating an emergency response.
- **Real-Time Metrics**: Displays the current mode (Automatic), cycle time, and the number of cars waiting in each direction.
- **Manual Controls**: A button allows manual simulation of traffic for testing purposes.

## File Structure
- **`index.html`**: The HTML file defines the layout of the project, including the intersection structure, traffic lights, metrics display, and simulation controls.
- **CSS Styles**: In-line styles manage the visual appearance of the roads, bypass lanes, vehicles, and traffic lights.
- **JavaScript Functionality**: JavaScript controls the vehicle movement, traffic light timing, and real-time metrics updating.

## Installation
1. Download or clone this repository.
2. Open `index.html` in a web browser to start the simulation.

## Usage
- **Start Simulation**: The simulation automatically begins upon loading `index.html`.
- **Simulate Traffic**: Press the "Simulate Traffic" button to add random vehicles to the intersection.
- **Observe Adaptive Timing**: Watch the adaptive timing adjust in real time based on traffic load, with updates every cycle (set initially to 30 seconds).

## Key Functions
- **`simulateTraffic()`**: Randomly generates cars and ambulances, displays real-time traffic metrics, and adjusts light timings.
- **`adjustCycleTime()`**: Calculates cycle time based on the number of cars waiting, setting `North-South` or `East-West` priority accordingly.
- **`updateLights()`**: Changes the traffic lights to allow vehicles to pass in the prioritized direction, clearing cars from the intersection.
- **`createAmbulance()`**: Simulates an ambulance entering the intersection, with a unique animation and prioritized movement across traffic.

## Animation Keyframes
- **`pulse`**: Pulsing effect for waiting cars to indicate idle status.
- **`flash`**: Flashing effect for ambulances to simulate emergency lights.
- **Movement Animations**:
  - `moveTopToBottom`, `moveBottomToTop`, `moveLeftToRight`, `moveRightToLeft`: Animates cars and ambulances moving across the intersection.

## Future Improvements
- Add manual control over traffic light timing modes (e.g., “Rush Hour” mode).
- Implement priority override when ambulances approach.
- Develop a system to detect traffic jams and dynamically adjust lanes or provide warnings.

## License
This project is for educational purposes and does not include any warranty. It can be freely used or modified under the terms of the MIT License.
