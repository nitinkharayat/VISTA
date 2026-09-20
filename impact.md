# VISTAX — Technical Impact Report
## Bailadila, NMDC | Mine Vehicle Safety in Fog & Low-Visibility Conditions

**Document purpose:** Evidence-backed description of expected operational impact, measurable pilot KPIs, and financial modelling for VISTAX at NMDC's Bailadila operations.

**Status:** Planning / pilot-validation document. VISTAX impact values below are **modelled estimates, not historical audited VISTAX results**.

---

## 1. Problem Context

Smart India Hackathon 2026 Problem Statement **SIH26007** is sponsored by the **Ministry of Steel** and concerns safe and efficient operation of mine vehicles in fog and low-visibility conditions in open-cast iron-ore mines.

The problem statement identifies Bailadila as the relevant mining context and states that, during monsoon conditions, haul-road visibility can become extremely low, affecting dumper movement, haul cycle time, fleet productivity, ore evacuation and production continuity.

The problem statement also identifies the need for technology that can improve operator situational awareness, assist vehicle guidance/collision avoidance, and support real-time monitoring and decision-making during adverse weather.

**Reference:** Smart India Hackathon 2026, PS 26007 — official SIH listing: https://www.sih.gov.in/sih2026PS

---

## 2. Bailadila / NMDC Baseline Facts

### FY 2024-25 production and sales

- **Bailadila Sector production:** 29.98 million tonnes (MT).
- **Chhattisgarh sector sales:** 30.81 MT.
- **NMDC total iron-ore production:** 44.07 MT.
- **NMDC total iron-ore sales:** 44.40 MT.
- **NMDC FY 2024-25 iron-ore sales value:** ₹22,803.40 crore.

The 29.98 MT and 30.81 MT Chhattisgarh figures are from NMDC's production and sales disclosure dated 1 April 2025.

**Source:** NMDC, "Details of Production & Sales of Iron Ore (Provisional) for and up to March 2025".
https://www.nmdc.co.in/cms-admin/Upload/Production_Sales_Prices_Documents/5769694fba1c42aaabf5b02afc78bad6_20250401155049736.pdf

The 44.07 MT production, 44.40 MT sales and ₹22,803.40 crore iron-ore sales value are reported in NMDC's FY 2024-25 annual report.

**Source:** NMDC Limited, Annual Report 2024-25.
https://www.nmdc.co.in/cms-admin/Upload/Annual_Report_Documents/38e8511b260c46fe9ab44c1948362166_20250807000209693.pdf

---

## 3. Relevant NMDC Cost Baseline

NMDC's FY 2024-25 consolidated financial statements disclose:

| Cost item | FY 2024-25 |
|---|---:|
| Petrol, Diesel, LDO & Lubricants | ₹210.09 crore |
| Repairs & Maintenance | ₹254.65 crore |
| Combined reference cost pool | **₹464.74 crore/year** |
| Monthly equivalent of combined pool | **₹38.73 crore/month** |

Important: these are **NMDC company-level disclosed costs**, not Bailadila-only costs and not proof of VISTAX savings.

**Source:** NMDC Limited, FY 2024-25 Annual Report, Note 2.36 (Consumption Stores & Spares) and Note 2.40 (Repairs & Maintenance).
https://www.nmdc.co.in/cms-admin/Upload/Annual_Report_Documents/38e8511b260c46fe9ab44c1948362166_20250807000209693.pdf

The same annual report shows FY 2024-25 consumption of approximately **27,143 kilolitres of diesel**, 1,892 kilolitres of LDO and 16 kilolitres of petrol in the disclosed fuel-consumption dataset.

**Source:** NMDC Sustainability / BRSR FY 2024-25.
https://www.nmdc.co.in/cms-admin/Upload/Environment_Sustainability_Documents/18ffd21ac9fa4c71a9578eb82909d301_20260131151221344.pdf

---

## 4. Existing NMDC Digital Baseline

VISTAX should **not** be presented as replacing NMDC's existing fleet-management capabilities.

NMDC has already implemented / advanced Fleet Management System capabilities at its Bailadila operations. The Ministry of Steel's FY 2024-25 Annual Report describes benefits including continuous driver-behaviour monitoring, route optimization, fuel-consumption reduction and reduced operating costs.

NMDC's FY 2024-25 Annual Report also lists **Vision Enhancement for Dumper Movement during Foggy Weather** among its digital initiatives and identifies Fleet Management System implementation in the Bailadila sector.

This supports positioning VISTAX as an **additional low-visibility safety and driver-assistance layer** that can complement existing FMS infrastructure.

**Sources:**

1. Ministry of Steel, Annual Report 2024-25, section on NMDC Fleet Management System.
https://steel.gov.in/sites/default/files/2025-04/Steel_English_AR_2024%20%281%29.pdf

2. NMDC Limited, Annual Report 2024-25, Digital Initiatives / Fleet Management / Vision Enhancement for Dumper Movement during Foggy Weather.
https://www.nmdc.co.in/cms-admin/Upload/Annual_Report_Documents/38e8511b260c46fe9ab44c1948362166_20250807000209693.pdf

---

## 5. VISTAX Solution Impact

### 5.1 Mine Vehicles

**Expected impact**

- Improved situational awareness under poor visibility using multiple sensor inputs.
- Multi-sensor collision-risk / obstacle detection using the proposed sensing stack.
- Position and motion context using GPS/DGPS and IMU.
- Local/offline vehicle-side alerts when network availability is limited.
- Sensor-health monitoring and fail-safe behaviour as part of the intended architecture.

**Evidence basis:** VISTAX website architecture and prototype description state camera, sonar, LiDAR, thermal, GPS/DGPS, IMU and communication hardware; the software architecture describes offline perception, sensor fusion, collision-risk detection, alerts and fail-safe operation.

**Source:** VISTAX project website.
https://bug-busters-hazel.vercel.app/

---

### 5.2 Driver / Operator

**Expected impact**

- Fused sensor information to supplement human visual awareness.
- Real-time advisory warnings for detected collision risks / hazards.
- Earlier warning in fog, darkness and other low-visibility conditions.
- Reduced dependence on direct visual detection alone.
- Driver-assistance support while the operator remains responsible for vehicle control.

**Safety posture:** VISTAX is currently described as **advisory / driver assistance, not autonomous vehicle control**.

**Source:** VISTAX project website.
https://bug-busters-hazel.vercel.app/

---

### 5.3 Mine Operations

**Expected impact**

- Better visibility into low-visibility operational events.
- Incident/event logging for review and root-cause analysis.
- Fleet-level analytics to identify utilization and downtime patterns.
- Centralized vehicle, alert and sensor-health information.
- Decision support for low-visibility operating conditions.
- Potential reduction in avoidable operational disruption, subject to pilot measurement.

**Source:** VISTAX project website; NMDC / Ministry of Steel digitalization references listed above.

---

## 6. Pilot KPIs — What Must Be Measured

The following metrics should be treated as **validation KPIs**, not as already-achieved results:

| KPI | Measurement method | Status / target |
|---|---|---|
| Detection reliability | Compare sensor detections with ground truth | VISTAX controlled-pilot target: **70–80%** |
| False-alert rate | False alerts per operating hour / vehicle | Measure in pilot |
| Alert latency | Sensor event to driver alert time | Measure in pilot |
| Haul cycle time | Baseline vs VISTAX-assisted operation | Measure in pilot |
| Downtime | Low-visibility interruption hours | Baseline vs pilot |
| Fleet utilization | Productive operating time / available time | Baseline vs pilot |
| Operator acceptance | Structured operator feedback | Measure in pilot |
| Near-miss / collision-risk events | Logged risk events per operating hour | Baseline vs pilot |
| Sensor availability | Percentage of time critical sensors are healthy | Measure in pilot |

**Source:** VISTAX project website, Future Validation section.
https://bug-busters-hazel.vercel.app/

---

## 7. Financial Impact Model — Bailadila / NMDC

### 7.1 Cost-saving model

Use the disclosed NMDC FY 2024-25 cost pool only as a **reference base**.

Combined annual reference pool:

`₹210.09 Cr + ₹254.65 Cr = ₹464.74 Cr/year`

Monthly reference pool:

`₹464.74 Cr / 12 = ₹38.73 Cr/month`

Illustrative efficiency range:

`3% × ₹38.73 Cr = ₹1.16 Cr/month`

`5% × ₹38.73 Cr = ₹1.94 Cr/month`

### Recommended website range

**Modelled cost-saving opportunity: ₹1.2–₹1.9 Cr/month**

**Important limitation:** This is not a Bailadila-only audited saving and not an observed VISTAX result. Before deployment, NMDC should provide Bailadila-specific cost-centre data so the cost-saving denominator can be replaced with actual site-level expenditure.

---

### 7.2 Revenue-value model

NMDC FY 2024-25 iron-ore sales:

`44.40 MT sold for ₹22,803.40 Cr`

Implied NMDC-wide average realization proxy:

`₹22,803.40 Cr / 44.40 MT ≈ ₹5,136/tonne`

This is a **company-wide average realization proxy**, not a Bailadila-specific price.

Bailadila/Chhattisgarh FY 2024-25 sales:

`30.81 MT/year ≈ 2.568 MT/month`

Illustrative incremental sellable-tonnage range:

`0.5% of 2.568 MT ≈ 12,840 tonnes/month`

`1.0% of 2.568 MT ≈ 25,680 tonnes/month`

At ~₹5,136/tonne:

`12,840 × ₹5,136 ≈ ₹6.6 Cr/month`

`25,680 × ₹5,136 ≈ ₹13.2 Cr/month`

### Recommended website range

**Modelled gross revenue value: ₹6.6–₹13.2 Cr/month**

**Important limitation:** This is **gross revenue value**, not incremental profit. It also assumes the additional tonnage is saleable and can be evacuated/processed without offsetting costs or constraints. The realization proxy is NMDC-wide, not Bailadila-only.

---

### 7.3 Combined modelled opportunity

**₹1.2–₹1.9 Cr/month cost-saving opportunity**

+

**₹6.6–₹13.2 Cr/month gross revenue-value opportunity**

=

## **₹7.8–₹15.1 Cr/month — Modelled Financial Opportunity**

This combined number is a **planning model**, not a historical VISTAX financial result.

---

## 8. Claims That Must NOT Be Presented as Actual Results

Do not present the following as already-proven VISTAX outcomes unless supported by signed-off mine pilot data:

- "Accident reduction of X%"
- "₹X crore/month actual savings"
- "₹X crore/month actual profit"
- "Continuous operation during all monsoon/fog conditions"
- "Zero accidents"
- "Guaranteed production increase"
- "Guaranteed downtime reduction"
- "100% detection"
- "Autonomous driving"

Use wording such as:

- **Expected impact**
- **Modelled opportunity**
- **Pilot target**
- **To be validated in field trial**
- **Baseline vs pilot measurement**

---

## 9. Recommended Website Impact Card

### IMPACT
**Measurable operational benefits for vehicles, drivers and mine operations in low-visibility conditions.**

### MINE VEHICLES
- Enhanced low-visibility situational awareness using camera + thermal sensing
- Multi-sensor obstacle / collision-risk detection using LiDAR, radar and distance sensing
- Position & motion monitoring using GPS/DGPS + IMU
- Local/offline safety alerts without cloud dependency

### DRIVER / OPERATOR
- Fused sensor view for improved driver awareness
- Real-time advisory alerts for detected collision risks / hazards
- Earlier warning in fog, darkness & poor visibility
- Driver-assistance support, with operator retaining vehicle control

### MINE OPERATIONS
- Reduced operational-disruption risk during low-visibility conditions
- Incident records, alerts & event logs for operational review
- Fleet analytics for identifying downtime and utilization patterns
- Centralized monitoring of vehicle status & sensor health

### PILOT KPIs
**Detection Reliability:** 70–80% target  |  **False Alert Rate:** To be measured  |  **Alert Latency:** To be measured  |  **Downtime / Cycle Time:** Baseline vs pilot  |  **Operator Feedback:** Pilot assessment

---

## 10. Recommended Technical Report Link

Use this label on the website:

**TECHNICAL IMPACT REPORT**  
*Bailadila, NMDC — Evidence, Financial Model & Validation Plan*

Button text:

**View Full Technical Report →**

Recommended note below the button:

> **Data basis:** NMDC FY 2024-25 disclosures + official Ministry of Steel references + VISTAX project architecture and explicitly stated pilot assumptions. Projected values are planning estimates, not historical VISTAX savings.

---

## 11. Primary References

### Government / PSU sources

1. **NMDC Limited — Annual Report 2024-25**  
   https://www.nmdc.co.in/cms-admin/Upload/Annual_Report_Documents/38e8511b260c46fe9ab44c1948362166_20250807000209693.pdf

2. **NMDC Limited — Production & Sales of Iron Ore, March 2025 disclosure**  
   https://www.nmdc.co.in/cms-admin/Upload/Production_Sales_Prices_Documents/5769694fba1c42aaabf5b02afc78bad6_20250401155049736.pdf

3. **Ministry of Steel — Annual Report 2024-25**  
   https://steel.gov.in/sites/default/files/2025-04/Steel_English_AR_2024%20%281%29.pdf

4. **NMDC — Sustainability / BRSR FY 2024-25 fuel-consumption data**  
   https://www.nmdc.co.in/cms-admin/Upload/Environment_Sustainability_Documents/18ffd21ac9fa4c71a9578eb82909d301_20260131151221344.pdf

5. **Government of India Forest / FAC record citing Bailadila FY 2024-25 production and 40-day production stoppage due to industrial relations**  
   https://forestsclearance.nic.in/writereaddata/FAC_Minutes/6119121212151document%2824%29.pdf

6. **Smart India Hackathon 2026 problem statement portal**  
   https://www.sih.gov.in/sih2026PS

### Project source

7. **VISTAX — Mine Vehicle Safety, SIH 2026 PS 26007**  
   https://bug-busters-hazel.vercel.app/

---

## 12. Source Interpretation Rules

- **Actual / disclosed:** NMDC or Government source explicitly reports the value.
- **Calculated:** Derived mathematically from disclosed values; the formula is shown.
- **Modelled:** Planning assumption applied to a disclosed baseline.
- **Target:** Intended pilot performance threshold, not achieved performance.
- **Expected impact:** Engineering hypothesis requiring field validation.
