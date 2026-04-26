# SensorLogger-

## Overview

SensorLogger treats my laptop as a multi-channel sensor array.

The program logs multiple sensor channels every 100 milliseconds, stores the data in a ring buffer, displays the values in a live terminal dashboard, and detects anomalies when any channel spikes.

This project is inspired by a hardware DAQ system like a National Instruments NI-DAQ board. A DAQ system collects multiple sensor signals using a shared timestamp and a fixed sample rate.

## Features

This project includes:

- Multi-channel sensor logging
- 100 ms sample interval
- Timestamped samples
- Ring buffer storage
- Live terminal dashboard using Rich
- CSV export
- Anomaly detection
- Camera motion detection using OpenCV optical flow
- CPU and memory monitoring using psutil

## Sensor Channels

The program logs these channels:

1. Microphone RMS
2. Camera motion magnitude
3. CPU usage percentage
4. Memory usage percentage
5. Battery percentage or CPU temperature fallback

The 4th added sensor channel is:

```text
memory_percent
