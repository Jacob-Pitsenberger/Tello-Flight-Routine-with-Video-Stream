# Tello Flight Routine with Video Stream

Execute this Python script to have your Tello drone perform a basic flight routine while simultaneously streaming video from its forward-facing camera. It employs the `djitellopy` library for drone interaction, threading for managing concurrent operations, and `OpenCV` for handling video frames. This setup showcases the seamless integration of drone flight automation with real-time video processing in Python.

## Project Overview

The script orchestrates a flight routine for the Tello drone, including taking off, executing movements in various directions, performing rotations, and finally, landing. Concurrently, it streams live video captured by the drone's camera, displaying it in real time. This dual functionality is achieved through Python's threading mechanism, enabling seamless and concurrent drone flight control and video streaming.

## Key Features

- **Concurrent Flight Control and Video Streaming**: Utilizes Python threading to ensure that drone flight commands and video streaming occur simultaneously, providing a smooth and integrated user experience.
- **Defined Flight Maneuvers**: Executes a predefined flight pattern that includes taking off, moving in specific directions, rotating, and landing, offering comprehensive control over the drone's movements.
- **Live Video Streaming**: Employs the `OpenCV` library to display live video from the drone's camera, offering real-time visual feedback of the drone's surroundings.
- **Stream Readiness Signaling**: Implements a threading event to signal when the video stream is ready, ensuring that flight commands are executed only after the video stream has been successfully initiated.

## Dependencies

- `djitellopy`: A Python library for Tello drone control.
- `opencv-python`: The OpenCV library for real-time computer vision operations.

## Author
Jacob Pitsenberger - 2024
