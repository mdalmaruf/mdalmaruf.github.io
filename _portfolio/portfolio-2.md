---
title: "Faster Fog Computing based Over-the-air Vehicular Updates: A Transfer Learning Approach"
excerpt: |
    This project introduces a cutting-edge algorithm for vehicular over-the-air (OTA) updates leveraging fog computing, enhancing network durability and reducing communication delays compared to cloud-based solutions. The approach optimizes fog node usage based on regional traffic patterns to minimize handover and communication delays, backed by a machine learning model predicting communication delay. A European WiFi hotspot signal strength dataset and a 5G dataset validate the method, showing a significant increase in net reserve fog resources and a decrease in OTA update time.
    
    <br/> <img src='/images/portfolio/IntegrationMiddleware.png' alt='System Integration Middleware' style='width: 400px; display: inline-block;'>
    <br/>
    <div>
        <p><strong>System Integration Middleware:</strong> This diagram outlines the integration of different layers from cloud service providers down to embedded systems in a vehicular network for OTA updates.</p>
    </div>
collection: portfolio
---

## Abstract
> Fog computing is a promising option for time-sensitive vehicular over-the-air (OTA) updates. Our proposed algorithm, based on traffic pattern analysis, optimizes fog node utilization to reduce delays and resource over-provisioning. Demonstrated through a case study, the approach predicts OTA update time by considering handover delay, propagation delay, transmission rate, and vehicular mobility.

## Full Paper: [Download](https://ieeexplore.ieee.org/abstract/document/9496152)

## Supplemental Materials: [Download](https://github.com/mdalmaruf/OTA-Update/blob/c480ca2d180b516a0f7261070bd52e4454c469dc/Faster%20Fog%20Computing%20OTA%20Update-Transfer%20Learning%20Approach%20(Supplemental%20Materials).pdf)

> Supplemental materials are available in the repository. These include detailed descriptions of the methodologies and additional results supporting the study. [PDF](https://github.com/mdalmaruf/OTA-Update/blob/c480ca2d180b516a0f7261070bd52e4454c469dc/Faster%20Fog%20Computing%20OTA%20Update-Transfer%20Learning%20Approach%20(Supplemental%20Materials).pdf)

## Simulation and Testbed Details

### Simulation
- Executed OTA update time prediction via Mininet-WiFi simulations considering factors like handover and propagation delay.

### Testbed
- Implemented a networked testbed with fog nodes and vehicles as VMs, using QEMU for ARM hardware emulation. Uptane framework integrated for OTA updates, with network connections established via a high-speed wireless router.

<a href="https://github.com/mdalmaruf/OTA-Update" style="color:#52adc8;"><strong>View the project on GitHub ![GitHub](Images/github-icon.png)</strong></a>
