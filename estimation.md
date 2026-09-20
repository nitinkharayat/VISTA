# VISTAX — Hardware Cost Estimation Report

**Project:** VISTAX — Mine Vehicle Safety for Fog and Low Visibility
**SIH Problem Statement:** 26007
**Estimate Date:** September 2026
**Currency:** Indian Rupees (INR)

---

# 1. Our Prototype Cost

The VISTAX website shows the prototype architecture using **ESP8266, Arduino, camera, sonar, LiDAR, thermal, GPS/DGPS, IMU and communication hardware**. The physical prototype shown on the website is intended as a college/SIH demonstration system rather than a production mining installation.

**Important:** The website does not publish exact individual component prices, so the following is an **estimated prototype BOM** based on the hardware categories shown on the website and typical student-development hardware.

| Hardware                                  |  Qty. | Estimated Rate | Estimated Cost |
| ----------------------------------------- | ----: | -------------: | -------------: |
| ESP8266 development module                |     1 |           ₹500 |           ₹500 |
| Arduino development board                 |     1 |           ₹700 |           ₹700 |
| RGB camera module                         |     1 |         ₹1,500 |         ₹1,500 |
| 4 m ultrasonic/sonar sensor               |     1 |           ₹650 |           ₹650 |
| Low-cost LiDAR distance sensor            |     1 |         ₹3,500 |         ₹3,500 |
| Prototype thermal sensor/module           |     1 |         ₹4,000 |         ₹4,000 |
| GPS module                                |     1 |           ₹900 |           ₹900 |
| IMU module                                |     1 |           ₹300 |           ₹300 |
| Wireless communication module             |     1 |         ₹1,200 |         ₹1,200 |
| DC power regulation/protection            | 1 set |         ₹1,000 |         ₹1,000 |
| Small display / status interface          |     1 |         ₹2,500 |         ₹2,500 |
| Buzzer + warning LED/strobe               |     1 |           ₹500 |           ₹500 |
| Wiring, connectors and terminals          | 1 set |         ₹1,500 |         ₹1,500 |
| Prototype enclosure / mould / fabrication |     1 |         ₹3,000 |         ₹3,000 |
| Sensor brackets and mounting hardware     | 1 set |         ₹1,500 |         ₹1,500 |
| PCB / perfboard / connectors              | 1 set |           ₹500 |           ₹500 |
| Battery / power supply                    |     1 |         ₹1,500 |         ₹1,500 |
| **TOTAL ESTIMATED COLLEGE PROTOTYPE**     |       |                |    **₹25,150** |

## Prototype Cost

> **Estimated college-level prototype cost: approximately ₹25,000–₹30,000**

This estimate includes the sensors, controller boards, wiring, power electronics, enclosure/mould fabrication, mounts and warning hardware.

The processing computer can be an **existing laptop/PC/tablet**, so it is not included as a new hardware purchase in this college-level estimate.

### Prototype sensor limitation

The **4 m ultrasonic/sonar sensor is suitable for demonstrating short-range distance sensing**, but it should **not be presented as the primary ranging technology for a real mining haul vehicle**.

Its role in the VISTAX prototype is therefore:

> **Our prototype / proof-of-concept distance sensing**

and not:

> **Production mine-vehicle ranging system**

---

# 2. Real-World Mine Implementation Cost

For actual mining deployment, the hardware must be changed from low-cost demonstration components to **industrial, ruggedized and vehicle-integrated hardware**.

The most important change is the ranging system:

> **4 m ultrasonic sonar → 77–81 GHz industrial radar**

Radar is more appropriate as the primary ranging technology for a mine vehicle because the system must operate over substantially greater distances and under difficult visibility conditions.

The real deployment should also use industrial thermal sensing, rugged cameras, RTK GNSS, industrial IMU, production-grade edge computing, protected vehicle power, sealed cabling, safety hardware and a rugged enclosure.

The detailed project hardware study gives the following component planning ranges and selected benchmark prices.

## Real-World Hardware BOM

| Hardware                                            |  Qty. | Estimated Rate | Estimated Cost |
| --------------------------------------------------- | ----: | -------------: | -------------: |
| 77–81 GHz industrial radar                          |     1 |        ₹60,000 |        ₹60,000 |
| Industrial thermal camera                           |     1 |      ₹1,50,000 |      ₹1,50,000 |
| Industrial IP67 front RGB camera                    |     1 |        ₹12,000 |        ₹12,000 |
| Industrial rear RGB camera                          |     1 |         ₹8,000 |         ₹8,000 |
| Industrial 3D LiDAR                                 |     1 |      ₹4,00,000 |      ₹4,00,000 |
| RTK GNSS receiver                                   |     1 |        ₹26,000 |        ₹26,000 |
| Dual RTK GNSS antennas                              |     2 |         ₹2,500 |         ₹5,000 |
| Industrial IMU                                      |     1 |        ₹25,000 |        ₹25,000 |
| NVIDIA Jetson Orin NX-class edge computer           |     1 |      ₹1,00,000 |      ₹1,00,000 |
| CAN / J1939 interface                               |     1 |        ₹10,000 |        ₹10,000 |
| Industrial 4G router                                |     1 |        ₹15,000 |        ₹15,000 |
| Industrial Ethernet switch                          |     1 |        ₹12,000 |        ₹12,000 |
| Industrial safety relay                             |     1 |        ₹14,000 |        ₹14,000 |
| Industrial emergency stop                           |     1 |         ₹2,500 |         ₹2,500 |
| Buzzer + strobe warning beacon                      |     1 |         ₹5,000 |         ₹5,000 |
| Rugged driver display                               |     1 |        ₹15,000 |        ₹15,000 |
| 24 V industrial DC UPS                              |     1 |         ₹8,000 |         ₹8,000 |
| Industrial DC/DC converter                          |     1 |         ₹8,000 |         ₹8,000 |
| Power protection, TVS, fuses and distribution       | 1 set |        ₹10,000 |        ₹10,000 |
| IP65/IP67 industrial enclosure                      |     1 |        ₹20,000 |        ₹20,000 |
| Industrial M12/M8 cabling and connectors            | 1 set |        ₹25,000 |        ₹25,000 |
| Rugged sensor mounts + vibration isolation + guards | 1 set |        ₹20,000 |        ₹20,000 |
| Sensor cleaning / air-purge provision               | 1 set |        ₹20,000 |        ₹20,000 |
| UWB worker tags + anchors                           | 1 set |        ₹40,000 |        ₹40,000 |
| Production enclosure tooling / fabrication          |     1 |        ₹50,000 |        ₹50,000 |
| Vehicle installation + calibration + integration    |     1 |      ₹1,00,000 |      ₹1,00,000 |
| Spare hardware / replacement allowance              | 1 set |        ₹50,000 |        ₹50,000 |
| **TOTAL ESTIMATED REAL-WORLD IMPLEMENTATION**       |       |                | **₹12,10,500** |

The hardware study supports the underlying planning ranges for radar, thermal, LiDAR, GNSS, IMU, communications, compute, safety hardware, enclosure, cabling and mounting.

## Real-World Implementation Cost

> **Estimated field implementation: approximately ₹12–15 lakh per mining vehicle**

The estimate can become substantially higher if a higher-end thermal camera, additional radar units, certified safety hardware, multiple 3D LiDAR units or mine-specific qualification is required.

---

# 3. Cost Comparison

| Deployment Stage                   |          Approximate Cost |
| ---------------------------------- | ------------------------: |
| **College/SIH Prototype**          |       **₹25,000–₹30,000** |
| **Real-World Mine Implementation** | **₹12–15 lakh / vehicle** |

### Main hardware transition

| College Prototype             | Real Mine Implementation             |
| ----------------------------- | ------------------------------------ |
| 4 m ultrasonic sonar          | 77–81 GHz industrial radar           |
| Hobby/student LiDAR           | Industrial LiDAR                     |
| Prototype thermal sensor      | Industrial thermal camera            |
| Development-board electronics | Rugged/industrial electronics        |
| Basic enclosure               | IP65/IP67 rugged enclosure           |
| Simple wiring                 | Sealed industrial wiring harness     |
| Student mounting              | Vibration-resistant vehicle mounting |
| Existing laptop/PC            | Dedicated edge-computing unit        |
| Basic power supply            | Protected vehicle power system       |
| Demonstration safety alarm    | Engineered safety hardware           |
| Controlled testing            | Mine-field validation                |

---

# 4. Why the Two Costs Are Very Different

The college prototype is designed to **prove the concept at low cost**.

The real mining implementation is designed to **operate on an actual mining vehicle**, where longer detection range, harsh environmental conditions, vibration, dust, water ingress, electrical transients, sensor contamination and safety-system reliability become important.

Therefore, the cost increase is mainly caused by:

* industrial radar replacing short-range sonar;
* industrial thermal imaging;
* rugged LiDAR;
* vehicle-grade compute;
* industrial networking;
* protected power electronics;
* IP-rated enclosure;
* industrial connectors and wiring;
* vibration-resistant mounting;
* safety hardware;
* calibration and vehicle integration;
* spare hardware.

---

# 5. Important Position of Sonar

### Prototype

The sonar is retained because it provides an inexpensive way to demonstrate the distance-sensing and sensor-fusion concept.

### Real Mine

The sonar should **not be treated as the main vehicle-ranging sensor**.

The real implementation uses:

> **Radar as the primary long-range ranging sensor**

with:

> **Thermal + RGB + LiDAR + GNSS + IMU**

providing complementary information.

This is consistent with the project's hardware study, which identifies ultrasonic sensing as a close-range option and keeps radar as the stronger primary ranging approach.

---

# 6. Scope of the Estimates

## College Prototype Cost

The ₹25,000–₹30,000 estimate represents a **student/SIH proof-of-concept hardware build**.

It assumes:

* low-cost development boards;
* short-range sonar;
* prototype LiDAR;
* prototype thermal sensing;
* existing computing hardware;
* fabricated/3D-printed enclosure and mounts;
* basic wiring and power system.

## Real-World Cost

The ₹12–15 lakh estimate represents an **engineering-level field implementation**, not a certified production system.

Additional costs may arise from:

* OEM vehicle integration;
* mine-specific testing;
* certification/approval;
* environmental qualification;
* safety validation;
* fleet deployment;
* maintenance;
* production tooling;
* site-specific communications;
* additional redundant sensors.

---

# 7. Recommended Financial Statement

> **VISTAX College Prototype: ~₹25,000–₹30,000**

> **VISTAX Real-World Mine Implementation: ~₹12–15 lakh per vehicle**

### One-line presentation version

> **Low-cost college prototype: ~₹0.25–0.30 lakh | Industrial mine implementation: ~₹12–15 lakh/vehicle**

---

# 8. Source References

### VISTAX Project Website

https://bug-busters-hazel.vercel.app/

The website lists the prototype hardware architecture including ESP8266, Arduino, camera, sonar, LiDAR, thermal, GPS/DGPS, IMU, radar and communication hardware.

### VISTA Hardware-Finance Study

Project hardware-finance document containing the detailed component-selection study, planning ranges and costed prototype BOM.

### Engineering Cost Basis

All prices in this document are **estimation/benchmark values**, not final purchase quotations.

Before commercial implementation, vendor quotations and vehicle/OEM integration costs must replace the planning estimates.

---

# 9. Final Estimated Cost

| System                                    |      Total Estimated Cost |
| ----------------------------------------- | ------------------------: |
| **VISTAX College Prototype**              |       **₹25,000–₹30,000** |
| **VISTAX Real-World Mine Implementation** | **₹12–15 lakh / vehicle** |

**The prototype demonstrates the concept.
The real-world version replaces short-range demonstration hardware with industrial sensing and vehicle-grade infrastructure.**
