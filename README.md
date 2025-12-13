# Caffora: Kinetic Universe

Caffora Kinetic Universe is a real time hand tracked particle simulation that combines WebGL rendering with MediaPipe Hands. The system creates a reactive 3D particle universe that responds to natural hand gestures such as pinching, opening, closing, and lateral movement.

## Features

- 25,000 GPU rendered particles using THREE.Points
- Real time hand tracking via MediaPipe Hands
- Gesture driven camera zoom, rotation, and gravity wells
- Smooth interpolated motion using velocity, damping, and restoration forces
- Additive blended glow particles with dual color gradients
- Interactive HUD with animated status, credits, and controls
- Fully responsive fullscreen canvas

## Gesture Controls

- Open Hand  
  Resets camera to default position

- Close Hand (Fist)  
  Triggers hyper zoom into the particle field

- Move Hand Left or Right  
  Rotates the entire universe smoothly

- Pinch (Thumb + Index)  
  Creates a localized gravity well that attracts particles

## Tech Stack

- HTML5
- JavaScript (ES6)
- Three.js r128
- WebGL
- MediaPipe Hands
- Google Fonts (IBM Plex Mono)

## How to Run

1. Save the file as `index.html`
2. Open it in a modern browser with camera permissions enabled
3. Allow camera access when prompted
4. Use one hand in view of the camera for interaction

A secure context is recommended. Running via `localhost` or HTTPS improves camera reliability.

## Configuration

Core behavior is controlled through the `CONFIG` object:

- `particleCount`  
- `defaultCamZ`  
- `zoomCamZ`  
- `maxRotation`  
- `lerpSpeed`  

Particle physics tuning can be adjusted directly in the animation loop.

## System Status

The HUD displays real time system state:
- Camera initialization
- Active hand tracking
- Gesture detection feedback

## Notes

This project is an experimental visual engine intended for interactive art and exploration. Gesture detection thresholds are tuned for general lighting conditions and may require adjustment depending on camera quality and environment.

## License

MIT License
