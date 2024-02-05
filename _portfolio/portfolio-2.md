---
title: "Faster Fog Computing based Over-the-air Vehicular Updates: A Transfer Learning Approach"
excerpt: |
    Fog computing emerges as a vital solution for time-sensitive vehicular over-the-air (OTA) updates, offering enhanced network durability and lower communication delays compared to the cloud. Our algorithm optimizes fog node resources, reducing OTA update times and improving network efficiency. The application of machine learning for communication delay prediction and the strategic enabling and disabling of fog nodes based on traffic load underscore the system's innovative approach to OTA updates.
    
    <br/> <img src='/images/portfolio/IntegrationMiddleware.png' alt='System Integration Middleware' style='width: 400px; display: inline-block;'>
    <br/>
    <div>
        <p><strong>Key Features:</strong></p>
        <ul>
            <li><strong>Optimized Fog Node Utilization:</strong> Efficient allocation of fog resources based on traffic patterns, reducing over-provisioning and associated delays.</li>
            <li><strong>Machine Learning-Driven Delay Prediction:</strong> Accurate prediction of communication delays between fog nodes and vehicles, ensuring timely updates.</li>
            <li><strong>Enhanced Resource Allocation:</strong> Strategic enabling and disabling of fog nodes to match traffic load, maximizing network responsiveness.</li>
            <li><strong>Comprehensive Delay Analysis:</strong> Includes handover and propagation delays, transmission rates, and vehicular mobility to predict OTA update time.</li>
            <li><strong>Real-World Data Validation:</strong> Utilization of European WiFi hotspot and 5G datasets to confirm the effectiveness of the proposed approach.</li>
            <li><strong>Scalability Assessment:</strong> Examination of throughput performance with varying vehicle numbers and OTA update sizes, ensuring robust system scalability.</li>
            <li><strong>Testbed Corroboration:</strong> Verification of simulation performance with a real-world testbed, employing QEMU virtualization and the Uptane framework.</li>
        </ul>     
    </div>
collection: portfolio
---

## Abstract
> Fog computing is a promising option for time-sensitive vehicular over-the-air (OTA) updates. Our proposed algorithm, based on traffic pattern analysis, optimizes fog node utilization to reduce delays and resource over-provisioning. Demonstrated through a case study, the approach predicts OTA update time by considering handover delay, propagation delay, transmission rate, and vehicular mobility.

## Key Features
- **Optimized Fog Node Utilization**: Efficient allocation of fog resources based on traffic patterns, reducing over-provisioning and associated delays.
- **Machine Learning-Driven Delay Prediction**: Accurate prediction of communication delays between fog nodes and vehicles, ensuring timely updates.
- **Enhanced Resource Allocation**: Strategic enabling and disabling of fog nodes to match traffic load, maximizing network responsiveness.
- **Comprehensive Delay Analysis**: Includes handover and propagation delays, transmission rates, and vehicular mobility to predict OTA update time.
- **Real-World Data Validation**: Utilization of European WiFi hotspot and 5G datasets to confirm the effectiveness of the proposed approach.
- **Scalability Assessment**: Examination of throughput performance with varying vehicle numbers and OTA update sizes, ensuring robust system scalability.
- **Testbed Corroboration**: Verification of simulation performance with a real-world testbed, employing QEMU virtualization and the Uptane framework.

## Full Paper: [Download](https://ieeexplore.ieee.org/abstract/document/9496152)

## Supplemental Materials: [Download](https://github.com/mdalmaruf/OTA-Update/blob/c480ca2d180b516a0f7261070bd52e4454c469dc/Faster%20Fog%20Computing%20OTA%20Update-Transfer%20Learning%20Approach%20(Supplemental%20Materials).pdf)

> Supplemental materials are available in the repository. These include detailed descriptions of the methodologies and additional results supporting the study. [PDF](https://github.com/mdalmaruf/OTA-Update/blob/c480ca2d180b516a0f7261070bd52e4454c469dc/Faster%20Fog%20Computing%20OTA%20Update-Transfer%20Learning%20Approach%20(Supplemental%20Materials).pdf)

## Simulation and Testbed Details

### Simulation
- Executed OTA update time prediction via Mininet-WiFi simulations considering factors like handover and propagation delay.

### Testbed
- Implemented a networked testbed with fog nodes and vehicles as VMs, using QEMU for ARM hardware emulation. Uptane framework integrated for OTA updates, with network connections established via a high-speed wireless router.

<a href="https://github.com/mdalmaruf/OTA-Update" style="color:#52adc8;"><strong>View the project on GitHub ![GitHub](Images/github-icon.png)</strong></a>
