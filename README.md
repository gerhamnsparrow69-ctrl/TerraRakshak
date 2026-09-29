# TerraRakshak
TerraRakshak: an AI-assisted 4WD mine rescue rover for SIH 2026 (SIH26039). Three-tier modular design with a 12V drivetrain, a 6-sensor MQ gas array, thermal and night-vision perception, and RPLIDAR SLAM, all integrated on a Raspberry Pi 5 running ROS 2. Team MineCrafters.
TerraRakshak is a modular rover that enters underground mines ahead of rescue teams to report toxic gases, heat signatures and terrain in real time. Built by Team MineCrafters (Team ID 152475) for Smart India Hackathon 2026, problem statement SIH26039.

Architecture

Tier 1, power and drivetrain: 12V LiPo, 2x BTS7960 drivers, 4 encoders and an Arduino Nano, with isolated 12V and 5V buses.
Tier 2, gas array: MQ-2, MQ-4, MQ-7, MQ-8, MQ-135 and MQ-136 sensors on an Arduino Nano, powered through a star topology.
Tier 3, compute and vision: Raspberry Pi 5 as the ROS 2 master, an ESP32 with 4x MLX90640 thermal arrays, 4x night-vision cameras, an RPLIDAR A1M8 and a DHT22.

Repo contents: mechanical design (chassis, machining, assembly sequence), electrical wiring and GPIO maps, and software.
