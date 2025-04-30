# AAE6102-Asg2
# Task 1 – Differential GNSS Positioning

This repository contains a detailed comparative analysis of various GNSS techniques used in smartphone navigation, including Differential GNSS (DGNSS), Real-Time Kinematic (RTK), Precise Point Positioning (PPP), and PPP-RTK. The analysis explores the advantages and limitations of each technique across several critical dimensions.

## Table of Contents

- [Introduction](#introduction)
- [Techniques Overview](#techniques-overview)
- [Methodology](#methodology)
- [Comparative Analysis](#comparative-analysis)
  - [Accuracy and Precision](#accuracy-and-precision)
  - [Infrastructure and Service Dependency](#infrastructure-and-service-dependency)
  - [Convergence Time and Real-Time Usability](#convergence-time-and-real-time-usability)
  - [Cost and Practicality](#cost-and-practicality)
  - [Hardware and Complexity Requirements](#hardware-and-complexity-requirements)
  - [Environmental Robustness](#environmental-robustness)
- [Conclusion](#conclusion)
- [Contributing](#contributing)
- [License](#license)

## Introduction

With the growing demand for high-precision navigation in smartphones, GNSS technologies have evolved to offer better accuracy and reliability. This project examines several advanced techniques for smartphone integration, including DGNSS, RTK, PPP, and PPP-RTK.

## Techniques Overview

- **Differential GNSS (DGNSS):** Utilizes correction signals from ground-based reference stations or satellite-based augmentation systems to enhance standard GNSS accuracy.
- **Real-Time Kinematic (RTK):** Delivers centimeter-level positioning using carrier-phase measurements and real-time corrections from nearby base stations.
- **Precise Point Positioning (PPP):** Provides global high-accuracy positioning using precise satellite orbit and clock corrections without local base stations.
- **PPP-RTK:** Combines the global accessibility of PPP with rapid, centimeter-level convergence similar to RTK.

## Methodology

The analysis compares these techniques based on six critical dimensions: accuracy, infrastructure dependency, convergence and real-time usability, cost and practicality, hardware and complexity requirements, and environmental robustness.

## Comparative Analysis

### Accuracy and Precision

- **DGNSS:** Enhances standalone GNSS accuracy to approximately 1–5 meters.
- **RTK:** Offers exceptional centimeter-level accuracy (1–2 cm).
- **PPP:** Achieves decimeter to low-centimeter accuracy after convergence.
- **PPP-RTK:** Combines global corrections with regional enhancements for fast, centimeter-level precision.

### Infrastructure and Service Dependency

- **DGNSS:** Requires basic augmentation signals.
- **RTK:** Depends heavily on nearby base stations.
- **PPP:** Needs precise satellite correction data globally.
- **PPP-RTK:** Relies on regional and global correction sources.

### Convergence Time and Real-Time Usability

- **DGNSS:** Provides immediate corrections.
- **RTK:** Achieves convergence in seconds.
- **PPP:** Experiences long convergence times.
- **PPP-RTK:** Reduces convergence to 1–5 minutes.

### Cost and Practicality

- **DGNSS:** Often free or included by default.
- **RTK:** Involves significant operational costs.
- **PPP:** Basic services may be free; premium services may incur costs.
- **PPP-RTK:** Typically subscription-based.

### Hardware and Complexity Requirements

- **DGNSS:** Minimal additional hardware requirements.
- **RTK:** Requires dual-frequency GNSS chips.
- **PPP:** Relatively hardware-friendly.
- **PPP-RTK:** Demands sophisticated integration.

### Environmental Robustness

- **DGNSS:** Reasonably robust against mild obstructions.
- **RTK:** Highly sensitive to signal interruptions.
- **PPP:** More tolerant to variable environments.
- **PPP-RTK:** Offers improved robustness over RTK.

## Conclusion

Each GNSS technique presents distinct advantages and limitations for smartphone navigation. As smartphone GNSS hardware advances and correction service networks expand, PPP-RTK is expected to play a crucial role in enabling applications such as autonomous driving and augmented reality.

# Task 2 – GNSS in Urban Areas


# Task 3 – GPS RAIM (Receiver Autonomous Integrity Monitoring)



# Task 4 – LEO Satellites for Navigation




# Task 5 – GNSS Remote Sensing



