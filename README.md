# Self-Built Satellite Ground Station 🌍📡
In this project, I will take a personal approach to building a weather satellite receiving station, inspired by the official Raspberry Pi guide. The guide uses a Raspberry Pi 4 (4GB), but I will be using a Raspberry Pi 3 and an RTL-SDR dongle to receive live transmissions from NOAA weather satellites, while extending the original concept with a cloud-based data viewing system.

## Overview

In  a nutshell, the RTL-SDR captures radio signals transmitted by NOAA satellites as they pass overhead and decodes them into weather images and telemetry data. Unlike a standard setup, this project integrates an AWS-powered web platform to store, process, and visualise the received data in real time from anywhere.

## Hardware

* Raspberry Pi 4 (4GB)
* RTL-SDR USB dongle
* Suitable antenna, e.g. V-dipole tuned for NOAA frequencies (for my case, this will be a custom antenna for the setup)

## Features

* 📡 Real-time reception of NOAA satellite signals
* 🛰 Automatic decoding of weather images
* ☁️ Cloud integration using AWS for remote access
* 🌐 Web interface to view and manage received data
* 🔄 Continuous data pipeline from ground station to cloud

## How It Works

1. The Raspberry Pi listens for NOAA satellite passes using the RTL-SDR dongle.
2. Signals are recorded and decoded into images and data locally.
3. The processed output is uploaded to an AWS backend.
4. A custom website retrieves and displays the data for easy viewing and analysis.

## Improvements Over Base Project

* Remote accessibility via web dashboard
* Centralised data storage in the cloud
* Potential for scaling to multiple ground stations
* Enhanced usability compared to local-only setups

## Future Enhancements

* Live pass tracking and scheduling
* Multi-satellite support
* Mobile-friendly web interface
* Data analytics and historical comparisons

## Summary

This project demonstrates how a "lower-cost" Raspberry Pi setup can be extended into a fully connected satellite ground station with cloud capabilities, combining radio reception, data processing, and modern web technologies into one system.


## In this README file i'll also add my BOM ill be using and also a photo of the parts I have already 

* BOM (I'll put the parts which ill use for this, although there are many different alternatives)
* Raspberry Pi 3 Model B (1G)
*suitable Raspberry Pi power supply (check the official Raspberry Pi website for details)
*microSD card (16G)
*Card reader for the microSD to your pc/laptop
*USB Software Defined Radio (SDR) receiver (I'm used this NESDR Mini TV28T v2)
*5 metres of 8mm Microbore Copper Tube
*MCX Male to BNC Female RG316 Low Loss Pigtail Adapter 23.5cm Cable
*BNC Male to BNC Female RG58 Coax Cable (depents on where you put the rasberry pi for me it'll be connected to the antenna itself so 1m)
*1.5 metre length of white plastic 40mm waste pipe

*File or sandpaper
*Solder
*4 x 2mm by 8mm self-tapping screws (doesn't really matter tbh)

Here are some photos of what I require for the project that i attached to the project

<img width="1366" height="684" alt="BOM1" src="https://github.com/user-attachments/assets/3aac5a83-8bcb-442f-a7db-dce8539f93c3" />
<img width="1352" height="646" alt="BOM2" src="https://github.com/user-attachments/assets/25c339d5-942f-49c4-a7ba-16a02951aed7" />
<img width="1366" height="684" alt="BOM3" src="https://github.com/user-attachments/assets/a63fad83-2b72-4fa1-9223-b99742450e9b" />
<img width="1329" height="553" alt="BOM4" src="https://github.com/user-attachments/assets/6b5f5560-5f21-4c87-87ac-a7394444bb61" />

Also there's also a diagram of how the antenna should look like


<img width="1482" height="1244" alt="diagram for antenna" src="https://github.com/user-attachments/assets/41877e6b-8c6f-4333-8c77-b1cfd0f2159f" />


