# Denial of Service (DoS) Impact Analysis


---

## Overview

 
This repository documents a controlled cybersecurity laboratory exercise analysing the impact of Denial of Service (DoS) style traffic on a web server. The work was conducted as part of an academic cybersecurity lab environment to understand how different types of network traffic affect system performance and service availability.

The project evaluates how various traffic generation techniques influence CPU utilisation, server responsiveness, and application-level behaviour.

  

---

## Objectives

The main objectives of this laboratory exercise were:

* Analyse whether CPU utilisation can be influenced through packet generation parameters.
* Investigate the impact of SYN-based traffic on server performance.
* Compare the effects of SYN traffic and ICMP traffic.
* Observe how repeated HTTP requests affect application-layer behaviour.
* Understand the chain of events that leads to service degradation or unresponsiveness.

---

## Experimental Environment

### Tools Used

* Linux operating system
* **hping3** – packet generation and network testing
* **curl** – HTTP request generation
* Bash scripting
* Linux system monitoring utilities

---

## Methodology

### 1. Baseline Observation

### 2. SYN Traffic Generation

### 3. ICMP Traffic Testing

### 4. HTTP Request Simulation

### 5. Service Degradation Analysis

---

## Key Findings

The experiment produced several important observations:

* CPU utilisation could be influenced by adjusting packet interval and packet size.
* SYN-based traffic created greater pressure on system resources than ICMP traffic under similar conditions.
* Increasing network traffic resulted in noticeable degradation of HTTP service responsiveness.
* When system resources became heavily utilised, the server struggled to process incoming requests, eventually leading to service unavailability.

---

## Repository Structure

```
dos-impact-analysis/
│
├── docs/
│   ├── dos-lab-specification.pdf
│   └── dos-impact-analysis-report.pdf
│
└── notes/
│    └── ethical-use.md
├── .gitignore
├── LICENSE
├── README.md
```

---

## Ethical Use Notice

---

## Author

**Arka Paul**
BSc (Hons) Computer Science – Cyber Security
University of Greenwich
