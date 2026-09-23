# VISTAX — SIH Prototype Hardware Cost

**Project:** VISTAX — Mine Vehicle Safety for Fog and Low Visibility
**SIH Problem Statement:** 26007
**Market Price Reference:** September 2026
**Currency:** INR

| Hardware                           |  Qty. | Current Benchmark |          Cost |
| ---------------------------------- | ----: | ----------------: | ------------: |
| **ESP32 38-Pin Development Board** |     1 |              ₹439 |          ₹439 |
| ESP32-CAM / OV2640                 |     1 |              ₹635 |          ₹635 |
| HC-SR04 Ultrasonic Sensor          |     1 |               ₹69 |           ₹69 |
| VL53L1X ToF LiDAR Sensor           |     1 |              ₹865 |          ₹865 |
| MLX90640 Thermal Camera            |     1 |            ₹4,711 |        ₹4,711 |
| NEO-6M GPS Module                  |     1 |              ₹266 |          ₹266 |
| MPU-6050 IMU                       |     1 |              ₹154 |          ₹154 |
| HC-05 Bluetooth Module             |     1 |              ₹215 |          ₹215 |
| OLED Display                       |     1 |             ~₹200 |         ~₹200 |
| Buzzer + Warning LED               | 1 set |             ~₹100 |         ~₹100 |
| DC-DC Buck Converter               |     1 |             ~₹110 |         ~₹110 |
| Breadboard + Jumper Wires          | 1 set |             ~₹250 |         ~₹250 |
| 12 V Power Supply / Battery        |     1 |             ~₹500 |         ~₹500 |
| Mounting, Connectors & Misc.       | 1 set |             ~₹750 |         ~₹750 |
| **Estimated Prototype Total**      |       |                   | **≈ ₹10,259** |

**Practical prototype budget:** **₹10,000–₹12,000**

The listed ESP32, HC-SR04, VL53L1X, GPS, IMU, Bluetooth and MLX90640 prices are based on current India listings.


# 2. Real-World Mine Vehicle Implementation

The production system requires substantially more rugged hardware. The cost should therefore be based on **named engineering products where public prices are available**, while vendor-quotation items are clearly identified.

| Hardware                               | Product / Benchmark                          | Qty. | Current Listed Rate |            Cost |
| -------------------------------------- | -------------------------------------------- | ---: | ------------------: | --------------: |
| Radar                                  | TI IWR1843 76–81 GHz radar sensor*           |    1 |              ₹2,521 |          ₹2,521 |
| 3D LiDAR                               | Livox Mid-360                                |    1 |           ₹1,59,999 |       ₹1,59,999 |
| Thermal                                | FLIR Lepton 3.1R 160×120 module              |    1 |             ₹14,237 |         ₹14,237 |
| RGB Camera                             | TP-Link VIGI C220I IP67 PoE camera           |    2 |              ₹3,599 |          ₹7,198 |
| RTK GNSS                               | AeroAtoms Orbit Neo, ZED-F9P                 |    1 |             ₹23,499 |         ₹23,499 |
| RTK Antennas                           | GNSS high-gain antennas                      |    2 |              ₹2,650 |          ₹5,300 |
| Edge Computer                          | Seeed reComputer J4012, Jetson Orin NX 16 GB |    1 |         ₹1,18,681** |       ₹1,18,681 |
| Industrial Ethernet Switch             | Moxa EDS-205A                                |    1 |             ₹11,136 |         ₹11,136 |
| Safety Relay                           | ABB Sentry SSR10 24 VDC                      |    1 |             ₹19,389 |         ₹19,389 |
| Emergency Stop                         | Eaton RMQ-Titan IP67                         |    1 |              ₹5,189 |          ₹5,189 |
| Warning Beacon                         | RS PRO 24 V LED Beacon                       |    1 |              ₹4,879 |          ₹4,879 |
| Industrial DC UPS                      | PULS UB20.241, 24 V / 600 W                  |    1 |             ₹49,872 |         ₹49,872 |
| DC/DC Converter                        | G-energy 24 V → 12 V, 60 W                   |    1 |     ~₹590 incl. GST |           ~₹590 |
| IP67 Enclosure                         | RS PRO Polycarbonate IP67 enclosure          |    1 |             ₹11,983 |         ₹11,983 |
| Industrial M12 Cabling                 | RS PRO IP67 M12 cable/connector benchmark    |    6 |              ₹1,691 |         ₹10,149 |
| 4G Connectivity                        | Quectel EC25 LTE module benchmark            |    1 |             ₹10,919 |         ₹10,919 |
| **Publicly Priced Hardware Benchmark** |                                              |      |                     | **≈ ₹4,55,500** |

* The TI IWR1843 price is for the **76–81 GHz radar sensor device itself**, not a complete rugged mining-radar assembly. Mouser lists the device from ₹2,520.52 at quantity 1, while TI's ecosystem also includes complete evaluation boards.

** The reComputer J4012 listing includes the Jetson Orin NX 16 GB platform, carrier hardware and storage. A current India listing was ₹118,681 incl. GST when checked.

The Livox Mid-360 is currently listed at ₹159,999 in India.

The FLIR Lepton 3.1R 160×120 module is listed at ₹14,236.95, while the higher-cost FLIR TG267 industrial thermal camera is listed around ₹65,999.

The TP-Link VIGI C220I is IP67-rated and supports vehicle detection; current India listings are around ₹3,006–₹3,599 depending on the lens/listing.

The AeroAtoms Orbit Neo ZED-F9P RTK GNSS is listed at ₹23,499, with RTK antenna options separately available.

Moxa EDS-205A is currently listed at ₹11,136, the ABB SSR10 safety relay at ₹19,389, the Eaton IP67 emergency stop at ₹5,189, and the RS PRO 24 V LED beacon at ₹4,879.

The PULS UB20.241 industrial 24 V UPS is listed at ₹49,872.42, and the G-energy 24 V-to-12 V industrial converter is ₹499 before GST.

The selected RS PRO IP67 enclosure is ₹11,982.64 incl. GST, and an RS PRO IP67 M12 connector/cable benchmark is ₹1,691.47 per unit incl. GST.

---

# 3. Items That Require Vendor Quotation

The following should **not** be assigned an invented “exact market price” because the final cost depends on vehicle model, mounting requirements, environmental rating and integration scope:

| Item                                              | Cost Basis       |
| ------------------------------------------------- | ---------------- |
| Complete rugged 77–81 GHz mining radar assembly   | Vendor quotation |
| Industrial vehicle-grade IMU                      | Vendor quotation |
| Rugged driver display                             | Vendor quotation |
| Industrial 4G/5G router                           | Vendor quotation |
| CAN/J1939 vehicle interface                       | Vendor quotation |
| Sensor protection / air-purge system              | Vendor quotation |
| Vehicle-specific mounting and vibration isolation | Vendor quotation |
| Vehicle installation and calibration              | Vendor quotation |
| Mine-site testing and validation                  | Vendor quotation |
| Safety certification / compliance                 | Vendor quotation |

This distinction matters. A **₹2,500 radar chip is not a ₹2,500 mining radar system**. The chip needs antenna, RF design, processing, enclosure, power, connectors, software and vehicle integration. Pretending otherwise is precisely how cost reports become PowerPoint fiction.

---

# 4. Correct Real-World Cost Position

The publicly priced hardware benchmark is approximately:

> **₹4.5–₹5.0 lakh per vehicle before vehicle-specific integration**

After adding industrial integration, ruggedization, calibration, mounting, testing, spare hardware and quotation-based components:

> **Planning range: approximately ₹6–₹10 lakh per vehicle**

A higher-end configuration using premium thermal imaging, higher-grade LiDAR, multiple radars, certified safety equipment or additional redundancy can exceed this range.

Therefore, the earlier **₹12–15 lakh/vehicle** figure should be presented only as a **higher-end deployment scenario**, not as the single exact market price.

---

# 5. Cost Comparison

| Deployment Stage                                  |       Current Planning Cost |
| ------------------------------------------------- | --------------------------: |
| **VISTAX College/SIH Prototype**                  |         **₹23,000–₹25,000** |
| **Real-World Engineering Configuration**          |   **₹6–₹10 lakh / vehicle** |
| **Higher-End / Heavily Ruggedized Configuration** | **₹10–₹15+ lakh / vehicle** |

---

# 6. Main Prototype-to-Production Transition

| College / SIH Prototype   | Real-World Mine Deployment           |
| ------------------------- | ------------------------------------ |
| HC-SR04 ultrasonic sensor | 76–81 GHz radar / industrial ranging |
| Low-cost LiDAR            | Industrial 3D LiDAR                  |
| MLX90640 thermal array    | Industrial thermal imaging           |
| ESP8266 / Arduino         | Vehicle-grade embedded controllers   |
| Consumer/prototype camera | Rugged IP-rated camera               |
| Basic GPS                 | RTK GNSS                             |
| MPU-6050                  | Industrial IMU                       |
| Basic wiring              | Sealed industrial cabling            |
| Prototype enclosure       | IP-rated rugged enclosure            |
| Existing PC/laptop        | Dedicated edge AI computer           |
| Student mounts            | Vibration-resistant vehicle mounts   |
| Prototype power supply    | Protected vehicle power system       |
| Demonstration alarm       | Engineered safety hardware           |

---

# 7. Why the Cost Increases

The difference is primarily driven by:

**Range:** Short-range prototype sensing must be replaced by longer-range vehicle sensing.

**Ruggedization:** Mining environments introduce dust, rain, vibration, temperature variation and mechanical stress.

**Reliability:** Production systems need protected power, industrial connectors, enclosure protection and redundant sensing.

**Processing:** Real-time multi-sensor fusion and AI inference require dedicated edge computing.

**Vehicle Integration:** CAN/J1939 interfaces, mounting, calibration, networking and installation add engineering cost.

**Safety:** Production deployment requires engineered safety hardware and site-specific validation.

---

# 8. Financial Statement for Presentation

> **VISTAX Prototype:** ~₹23K–₹25K
> **Real-World Deployment:** ~₹6–₹10 lakh/vehicle
> **Higher-End Configuration:** ~₹10–₹15+ lakh/vehicle

**The prototype validates the sensing and AI concept using affordable development hardware. The production system upgrades the same architecture with industrial sensing, edge computing, ruggedized hardware, vehicle integration and safety infrastructure.**

---

# 9. Pricing Methodology

**Market-price basis:** Public India listings checked in September 2026.

**Included:** Current listed product prices for identifiable hardware.

**Excluded from “exact product price”:** Vendor-specific integration, certification, mine-site installation, calibration and custom engineering.

**Important:** Online electronics prices can change with stock, discounts, tax treatment, import costs and quantity. The figures should therefore be treated as **current market benchmarks**, while procurement should use final vendor quotations.

---

# 10. Key Product References

**Electronics / Prototype Components:** ElectronicsComp, Robu, Robocraze and other India electronics suppliers.

**Thermal Imaging:** ThinkRobotics / FLIR / DigiKey listings.

**LiDAR:** Livox / Indian robotics suppliers.

**RTK GNSS:** AeroAtoms / GenX India listings.

**Edge AI:** Seeed reComputer / NVIDIA Jetson Orin NX India listings.

**Industrial Networking & Safety:** Moxa, ABB, Eaton and RS India listings.

**Radar:** Texas Instruments IWR1843 76–81 GHz industrial radar sensor and associated evaluation hardware.
