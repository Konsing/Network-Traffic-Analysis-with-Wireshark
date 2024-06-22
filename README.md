# Network Traffic Analysis with Wireshark and Jupyter

This repository contains a project focused on analyzing network traffic using Wireshark and Jupyter Notebook. The project includes multiple packet capture (PCAP) files and a Jupyter Notebook for analyzing the captured data.

## Table of Contents
- [Introduction](#introduction)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
- [Analysis](#analysis)

## Introduction
This project demonstrates how to use Wireshark to capture network traffic and then analyze the captured data using a Jupyter Notebook. It includes several PCAP files capturing various network protocols and a Jupyter Notebook to perform detailed analysis.

## Project Structure
The project includes the following files:
- **1. Google.pcap**: Packet capture file for traffic to Google.
- **2. example.pcap**: Packet capture file for general example traffic.
- **3. httpforever.pcap**: Packet capture file for persistent HTTP connections.
- **4. FTP.pcap**: Packet capture file for FTP traffic.
- **5. SSH.pcap**: Packet capture file for SSH traffic.
- **Program.ipynb**: Jupyter Notebook containing the code for analyzing the captured network traffic.

## Getting Started

### Prerequisites
- Python 3.x
- Jupyter Notebook
- Wireshark
- tshark (command-line version of Wireshark)
- pandas

### Installation
1. Clone this repository:
   ```sh
   git clone https://github.com/yourusername/network-traffic-analysis.git
   cd network-traffic-analysis
   ```

2. Install the required Python packages:
   ```sh
   pip install jupyter pandas
   ```

3. Ensure Wireshark and tshark are installed on your system.

## Usage
1. **Capture Network Traffic**:
   - Use Wireshark or tshark to capture network traffic and save it as a PCAP file.
   - Example:
     ```sh
     tshark -i eth0 -w capture.pcap
     ```

2. **Analyze Captured Traffic**:
   - Open Jupyter Notebook:
     ```sh
     jupyter notebook
     ```
   - Open the `Program.ipynb` file in Jupyter.
   - Run the cells in the notebook to load and analyze the captured network traffic data.

## Analysis
The `Program.ipynb` notebook includes the following analyses:
- Parsing the PCAP files to extract HTTP, FTP, and SSH traffic.
- Analyzing traffic patterns, response times, and data transfer sizes.
- Visualizing the traffic data using graphs and charts.