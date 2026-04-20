# Landslide Detection System using mbed NXP LPC1768

A microcontroller-based landslide detection system built using the SW-420 vibration sensor and mbed NXP LPC1768, programmed in ARM Assembly. Developed as part of the Microprocessor subject at UTeM.

## Overview

Landslides are a frequent natural disaster in Malaysia, often with little warning. This system detects ground vibrations using the SW-420 sensor and alerts users via LED indicators — red for danger, green for stable.

## How It Works

- SW-420 vibration sensor continuously scans for ground vibration
- If vibration is **detected** → **Red LED turns ON** (dangerous condition)
- If vibration is **not detected** → **Green LED turns ON** (stable condition)

## Hardware Components

| Component | Description |
|---|---|
| mbed NXP LPC1768 | 32-bit ARM Cortex-M3 microcontroller @ 96MHz |
| SW-420 | Non-directional vibration sensor module |
| Red LED | Danger indicator |
| Green LED | Stable indicator |
| Resistors | Current limiting for LEDs |
| Breadboard | Circuit prototyping |

## Pin Configuration

| Component | Pin |
|---|---|
| SW-420 DO (output) | Pin 5 |
| Green LED | Pin 9 |
| Red LED | Pin 10 |

## Software

- **Language:** ARM Assembly
- **Tool:** Keil µVision
- **Logic:** Reads digital output from SW-420 at pin 5. Branches to stable or danger state based on HIGH/LOW input.

## Results

The system successfully demonstrated two states:
- Green LED ON when no vibration is detected (stable)
- Red LED ON when vibration is detected (dangerous)

## Project Report

See [PROJECT_REPORT.pdf](./PROJECT_REPORT.pdf) for full documentation including circuit diagrams, flowchart, and source code.

## Institution

Universiti Teknikal Malaysia Melaka (UTeM)  
Faculty of Electronic & Computer Engineering
