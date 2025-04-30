# AAE6102-Asg2
# Task 1 – Differential GNSS Positioning


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
##AI
The conversation with the AI is in the file Task1.txt



# Task 2 – GNSS in Urban Areas


# Task 3 – GPS RAIM (Receiver Autonomous Integrity Monitoring)



# Task 4 – LEO Satellites for Navigation




# Task 5 – GNSS Remote Sensing



