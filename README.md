# Denial of Service (DoS) Impact Analysis – Cybersecurity Lab

## Overview
This repository documents a controlled cybersecurity laboratory exercise analysing the impact of Denial of Service (DoS) style traffic on a web server. The work was conducted as part of an academic cybersecurity lab environment to understand how different types of network traffic affect system performance and service availability.

The project evaluates how various traffic generation techniques influence CPU utilisation, server responsiveness, and application-level behaviour.

## Objectives
The main objectives of this lab were:

- To evaluate whether CPU utilisation can be controlled through packet generation parameters.
- To analyse the effects of SYN-based traffic on a web server.
- To compare SYN traffic with ICMP-based traffic.
- To test application-layer pressure using repeated HTTP requests.
- To analyse the chain of events that lead to service degradation or failure.

## Experimental Environment
The testing was performed in a **controlled virtual lab environment** using Linux-based systems. All experiments were conducted on authorised machines specifically configured for cybersecurity training.

Typical tools used include:

- `hping3` – packet generation and network traffic testing
- `curl` – HTTP request generation
- Linux system monitoring tools (CPU and process monitoring)

## Methodology
The experiment consisted of multiple stages:

### 1. Baseline Measurement
Initial system performance was observed under normal conditions with no additional traffic.

### 2. Controlled SYN Traffic
SYN packets were generated at different rates to observe how CPU utilisation and service responsiveness changed.

### 3. ICMP Traffic Testing
ICMP packets were generated to compare their impact with SYN traffic under similar load conditions.

### 4. HTTP Request Loop
A scripted HTTP request loop was executed to simulate repeated client requests and observe application-layer behaviour.

### 5. Service Degradation Analysis
The system behaviour was analysed as utilisation increased to determine how and why the web service became unresponsive.

## Key Findings
The experiment produced several observations:

- CPU utilisation could be influenced by adjusting packet interval and packet size.
- SYN-based traffic had a stronger impact on server performance compared to ICMP traffic under similar conditions.
- Increasing network load resulted in significant degradation in HTTP service responsiveness.
- Under high load conditions, the web server became unable to process incoming requests, resulting in service unavailability.

## Repository Structure
