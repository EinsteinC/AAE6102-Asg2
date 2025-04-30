# AAE6102-Asg2
Task 1, 4, and 5 are assisted by GenAI model, and the Chatroom file and  links are as follows

Task1.txt

Task4: https://poe.com/s/bSRyHOKlhKenW5gWMxt8

Task5.txt

# Task 1 – Differential GNSS Positioning
#  Comparative Analysis of GNSS Positioning Techniques for Smartphone Navigation

## Introduction

The demand for precise navigation in smartphones is increasing, prompting advancements in Global Navigation Satellite System (GNSS) technologies to enhance accuracy and reliability. Several sophisticated techniques are being considered for smartphone integration, including Differential GNSS (DGNSS), Real-Time Kinematic (RTK), Precise Point Positioning (PPP), and PPP-RTK.

These methods each improve basic GNSS positioning in unique ways:

- **Differential GNSS (DGNSS):** Utilizes correction signals from ground-based reference stations or satellite-based augmentation systems to enhance standard GNSS accuracy, achieving improvements at the meter level.
- **Real-Time Kinematic (RTK):** Delivers centimeter-level positioning by employing carrier-phase measurements and real-time corrections from nearby base stations.
- **Precise Point Positioning (PPP):** Provides global high-accuracy positioning using precise satellite orbit and clock corrections without relying on local base stations, though it requires longer convergence times.
- **PPP-RTK:** Merges the global accessibility of PPP with the rapid, centimeter-level convergence of RTK by integrating wide-area and regional correction services.

This report introduces these techniques and systematically compares them based on six critical dimensions: accuracy, infrastructure dependency, convergence and real-time usability, cost and practicality, hardware and complexity requirements, and environmental robustness.

## Accuracy and Precision

- **DGNSS:** Enhances standalone GNSS accuracy from approximately 10 meters to about 1–5 meters, which is adequate for general navigation but insufficient for lane-level or high-precision needs.
- **RTK:** Offers exceptional centimeter-level accuracy (1–2 cm) by resolving carrier-phase ambiguities in real-time, making it suitable for applications like lane positioning and augmented reality.
- **PPP:** Achieves decimeter to low-centimeter accuracy after convergence. While better than DGNSS, its consistency under smartphone conditions is generally less than RTK.
- **PPP-RTK:** Combines global corrections with regional enhancements to achieve centimeter-level precision with faster initialization, providing an optimal balance for mobile real-time navigation.

## Infrastructure and Service Dependency

- **DGNSS:** Requires basic augmentation signals, either broadcast via satellites or regional stations.
- **RTK:** Heavily depends on nearby base stations and real-time data communication through cellular networks.
- **PPP:** Needs only precise satellite correction data, typically available globally through satellite broadcast or internet distribution, without local base station reliance.
- **PPP-RTK:** Relies on a network of regional and global correction sources, combining satellite corrections and ground network assistance, necessitating stable internet access.

## Convergence Time and Real-Time Usability

- **DGNSS:** Provides immediate corrections, offering real-time usability without convergence delay—ideal for continuous smartphone navigation.
- **RTK:** Achieves convergence in seconds after receiving corrections, ensuring seamless, real-time centimeter-level tracking.
- **PPP:** Experiences long convergence times, typically ranging from 5 to 30 minutes, which hinders real-time usability for smartphones.
- **PPP-RTK:** Reduces convergence to 1–5 minutes by quickly resolving ambiguities, making it practical for dynamic smartphone applications.

## Cost and Practicality

- **DGNSS:** Often free or included by default through public augmentation systems, with no extra subscription or hardware cost.
- **RTK:** Involves significant operational costs for correction service subscriptions and requires stable mobile data connectivity.
- **PPP:** Basic services may be free, but premium PPP services offering faster convergence and higher accuracy may incur costs.
- **PPP-RTK:** Typically subscription-based, especially for commercial-grade services (e.g., Trimble RTX, Qianxun SI), though costs are increasingly bundled into smartphone service plans.

## Hardware and Complexity Requirements

- **DGNSS:** Minimal additional hardware requirements. Current smartphones can easily leverage DGNSS corrections through standard single-frequency GNSS receivers.
- **RTK:** Requires dual-frequency (L1/L5) GNSS chips, advanced carrier-phase tracking algorithms, and robust antenna performance, supported only by high-end smartphones.
- **PPP:** Requires good GNSS signal quality but is relatively hardware-friendly compared to RTK, as it does not require ground-based reference station communication.
- **PPP-RTK:** Demands sophisticated integration, involving dual-frequency GNSS, continuous data reception, and rapid ambiguity resolution, challenging mid-range smartphone hardware.

## Environmental Robustness

- **DGNSS:** Reasonably robust against mild obstructions but degrades in dense urban canyons due to multipath and signal blockage.
- **RTK:** Highly sensitive to signal interruptions, cycle slips, and multipath, requiring open-sky conditions for optimal performance.
- **PPP:** More tolerant to variable environments because of global corrections, but multipath and atmospheric conditions still impact convergence.
- **PPP-RTK:** Offers improved robustness over RTK by leveraging wide-area corrections but still benefits from open-sky views for best performance.

## Conclusion

Each GNSS technique presents distinct advantages and limitations for smartphone navigation:

- **DGNSS** offers immediate and affordable improvements, suited for everyday applications.
- **RTK** provides the highest accuracy but faces barriers in cost, communication, and hardware complexity.
- **PPP** allows global high-accuracy navigation but is hindered by long convergence periods.
- **PPP-RTK** represents the best balance, offering fast, high-precision positioning with global coverage and is poised to become the mainstream solution for future smartphones.

As smartphone GNSS hardware continues to advance and correction service networks expand, PPP-RTK is expected to play a crucial role in enabling applications such as autonomous driving, pedestrian navigation, and augmented reality on handheld devices.

To further clarify the differences among the four GNSS techniques, the following table summarizes their key characteristics across critical performance dimensions.




# Task 2 – GNSS in Urban Areas


# Task 3 – GPS RAIM (Receiver Autonomous Integrity Monitoring)



# Task 4 – LEO Satellites for Navigation
# Challenges of Using LEO Communication Satellites for GNSS Navigation

## Introduction
Low Earth Orbit (LEO) satellites, typically operating at altitudes between 160 km and 2,000 km, are widely used for communication services such as global internet coverage (e.g., Starlink, OneWeb). However, their potential use for Global Navigation Satellite System (GNSS) navigation presents unique challenges. While LEO satellites offer advantages like lower latency and stronger signal strength compared to traditional Medium Earth Orbit (MEO) GNSS satellites (e.g., GPS, Galileo), several technical and operational difficulties must be addressed before they can reliably support navigation. This essay explores the key challenges of using LEO communication satellites for GNSS navigation, including orbital dynamics, signal processing, time synchronization, and regulatory constraints.

## 1. High Orbital Dynamics and Coverage Limitations
### (a) Rapid Satellite Movement and Short Visibility Periods
LEO satellites move at approximately 7.8 km/s, completing an orbit every 90 minutes. This results in a single satellite being visible to a ground user for only 10–20 minutes, necessitating frequent signal handovers between satellites and complicating receiver tracking and positioning stability.

### (b) Constellations Require Massive Scale for Continuous Coverage
LEO satellites have a much smaller coverage footprint, requiring hundreds or even thousands of satellites for uninterrupted navigation services. For example, Starlink's communication constellation plans to deploy over 40,000 satellites, necessitating additional modifications for navigation support.

## 2. Signal Processing Challenges
### (a) Severe Doppler Shift Effects
LEO satellites introduce significant Doppler frequency shifts in their signals, demanding advanced signal processing algorithms and higher computational power for receivers to compensate for rapid frequency changes.

### (b) Non-Navigation-Optimized Signals
Modifying LEO communication satellites for GNSS requires new signal structures, additional power allocation for navigation signals, and interference management to prevent conflicts between navigation and communication signals.

## 3. Time Synchronization and Clock Stability
### (a) Frequent Clock Corrections Needed
LEO satellites experience higher orbital perturbations, requiring much more frequent clock adjustments (possibly hourly) for precise time synchronization, increasing system complexity.

### (b) Dependency on Inter-Satellite Links
Real-time inter-satellite links may be required to maintain synchronization, adding further technical challenges to LEO-based navigation systems.

## 4. Atmospheric and Environmental Interference
### (a) Ionospheric Delay Variations
Calibrating ionospheric delay models for LEO signals is challenging due to the rapid motion of satellites, requiring dynamic real-time corrections for accurate navigation.

### (b) Urban Multipath and Signal Blockage
LEO signals are more susceptible to multipath interference and obstruction in urban environments, affecting positioning accuracy in critical areas.

## 5. Orbital Maintenance and Space Debris Risks
### (a) Atmospheric Drag and Orbital Decay
LEO satellites require periodic orbital maintenance to counteract atmospheric drag and prevent orbital decay, ensuring positioning accuracy and service continuity.

### (b) Collision Risks from Space Debris
Active debris avoidance maneuvers are necessary to mitigate collision risks in the densely populated LEO region, safeguarding navigation constellation operations.

## 6. Regulatory and Standardization Challenges
### (a) Frequency Allocation Conflicts
Coordinating dedicated navigation frequencies in LEO with existing spectrum users requires international coordination through the ITU, potentially facing resistance from other services.

### (b) Military and Political Considerations
National security concerns and regulatory restrictions may impact the global acceptance of LEO-based navigation systems, necessitating diplomatic agreements for widespread adoption.

## Conclusion
LEO communication satellites offer potential benefits for GNSS navigation but face significant challenges in orbital dynamics, signal processing, time synchronization, atmospheric effects, and regulatory compliance. Overcoming these obstacles will require advancements in onboard technology, algorithms, and international cooperation. Successful resolution could open new opportunities for LEO-based navigation in urban areas, autonomous vehicles, and emergency scenarios. However, until these challenges are addressed, traditional MEO GNSS systems like GPS and Galileo will remain the primary choice for reliable global positioning.



# Task 5 – GNSS Remote Sensing



