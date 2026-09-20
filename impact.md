# VISTAX — Technical Impact Report
## Bailadila, NMDC | Mine Vehicle Safety in Fog & Low-Visibility Conditions

Document purpose: Evidence-backed description of the expected operational impact of VISTAX, the measurable pilot KPIs, the financial modelling approach, and the validation plan for mine-vehicle safety at NMDC Bailadila.

**Status: Planning / pilot-validation document**

> VISTAX impact values in this document are expected impacts, pilot targets, calculated values, or modelled scenarios. They are not historical audited VISTAX results.

---

## 1. Problem Context

Smart India Hackathon 2026 Problem Statement SIH26007 is sponsored by the Ministry of Steel and concerns the safe and efficient operation of mine vehicles in fog and low-visibility conditions in open-cast iron-ore mines.

The problem context identifies adverse visibility as a factor that can affect dumper movement, haul cycle time, fleet productivity, ore evacuation and production continuity.

The problem statement also identifies the need for technology that can improve operator situational awareness, support vehicle guidance / collision-risk awareness, and provide real-time monitoring and decision support during adverse weather.

Reference:

Smart India Hackathon 2026 — Problem Statement SIH26007  
https://www.sih.gov.in/sih2026PS

---

## 2. Bailadila / NMDC Baseline Facts

### FY 2024-25 production and sales

NMDC's disclosed FY 2024-25 figures include:

| Metric | FY 2024-25 |
|---|---:|
| Bailadila / Chhattisgarh sector production | 29.98 MT |
| Chhattisgarh sector sales | 30.81 MT |
| NMDC total iron-ore production | 44.07 MT |
| NMDC total iron-ore sales | 44.40 MT |
| NMDC iron-ore sales value | ₹22,803.40 crore |

The 29.98 MT production and 30.81 MT sales figures are from NMDC's production and sales disclosure dated 1 April 2025.

The 44.07 MT production, 44.40 MT sales and ₹22,803.40 crore sales value are reported in NMDC's FY 2024-25 Annual Report.

### Source

NMDC — Details of Production & Sales of Iron Ore for and up to March 2025  
https://www.nmdc.co.in/cms-admin/Upload/Production_Sales_Prices_Documents/5769694fba1c42aaabf5b02afc78bad6_20250401155049736.pdf

NMDC Limited — Annual Report 2024-25  
https://www.nmdc.co.in/cms-admin/Upload/Annual_Report_Documents/38e8511b260c46fe9ab44c1948362166_20250807000209693.pdf

---

## 3. Historical Operational Disruption Context

A Government of India forest-clearance record states that FY 2024-25 Bailadila production was affected by a 40-day stoppage associated with Industrial Relations (IR).

The same record indicates that production otherwise would have reached approximately 90% of total production capacity.

This event is included only as historical operational context.

**It must not be treated as a VISTAX-addressable loss or as evidence of a VISTAX production benefit**, because the documented cause was Industrial Relations rather than low visibility or vehicle collision risk.

### Source

Government of India Forest / FAC record:

https://forestsclearance.nic.in/writereaddata/FAC_Minutes/6119121212151document%2824%29.pdf

---

## 4. Relevant NMDC Cost Baseline

NMDC's FY 2024-25 financial disclosures report the following company-level cost items:

| Cost item | FY 2024-25 |
|---|---:|
| Petrol, Diesel, LDO & Lubricants | ₹210.09 crore |
| Repairs & Maintenance | ₹254.65 crore |
| Combined reference pool | ₹464.74 crore/year |
| Simple monthly equivalent | ₹38.73 crore/month |

These figures are **NMDC company-level reference values**, not Bailadila-only costs and not proof of VISTAX savings.

They are therefore suitable for sensitivity analysis only.

### Fuel-consumption reference

NMDC's FY 2024-25 disclosed fuel-consumption data includes approximately:

- Diesel: 27,143 kilolitres
- LDO: 1,892 kilolitres
- Petrol: 16 kilolitres

These quantities provide context for the scale of NMDC's fuel consumption but do not establish a VISTAX-attributable saving.

### Sources

NMDC Limited — Annual Report 2024-25  
https://www.nmdc.co.in/cms-admin/Upload/Annual_Report_Documents/38e8511b260c46fe9ab44c1948362166_20250807000209693.pdf

NMDC — Sustainability / BRSR FY 2024-25  
https://www.nmdc.co.in/cms-admin/Upload/Environment_Sustainability_Documents/18ffd21ac9fa4c71a9578eb82909d301_20260131151221344.pdf

---

## 5. Existing NMDC Digital Baseline

VISTAX should be positioned as an **augmentation layer**, not as a replacement for NMDC's existing digital fleet-management systems.

NMDC has already implemented / advanced Fleet Management System capabilities at Bailadila operations.

The Ministry of Steel Annual Report describes NMDC FMS capabilities and benefits including driver-behaviour monitoring, route optimization, fuel-consumption management and operating-cost control.

NMDC's FY 2024-25 Annual Report also identifies:

> Vision Enhancement for Dumper Movement during Foggy Weather

among its digital initiatives and identifies Fleet Management System implementation in the Bailadila sector.

### VISTAX positioning

VISTAX is designed to complement existing FMS capabilities by concentrating on the low-visibility safety problem:

1. Forward hazard perception under poor visibility.
2. Collision-risk awareness for vehicle operators.
3. Multi-sensor perception and ranging context.
4. Local vehicle-side advisory alerts when connectivity is weak.
5. Event logging for visibility and near-miss situations.
6. Linking safety events with fleet and operational data.

VISTAX therefore acts as a **low-visibility safety and driver-assistance layer around the existing digital mine ecosystem**.

### Sources

Ministry of Steel — Annual Report 2024-25  
https://steel.gov.in/sites/default/files/2025-04/Steel_English_AR_2024%20%281%29.pdf

NMDC Limited — Annual Report 2024-25  
https://www.nmdc.co.in/cms-admin/Upload/Annual_Report_Documents/38e8511b260c46fe9ab44c1948362166_20250807000209693.pdf

---

## 6. VISTAX Solution Impact

### 6.1 Mine Vehicles

### Expected impact

- Improved situational awareness under poor visibility using multiple sensor inputs.
- Obstacle and collision-risk detection using the proposed sensing architecture.
- Position and motion context where GPS/DGPS and IMU are available.
- Local/offline vehicle-side warning when network availability is limited.
- Sensor-health monitoring and degraded-mode behaviour as part of the intended architecture.
- Event recording to support post-incident review and operational analysis.

### Technology status

To avoid overstating the current prototype, the technology stack is separated into demonstrated, prototype-integrated, and future-validation components.

**Currently demonstrated / represented in the prototype:**

- Camera-based perception.
- Vehicle-side monitoring and warning workflow.
- Driver-assistance interface.
- Event / alert handling.
- Offline-capable software workflow.

**Proposed sensor-integration layer:**

- Thermal imaging.
- LiDAR / distance sensing.
- Sonar / ranging.
- GPS / DGPS.
- IMU.
- Additional industrial communication interfaces.

**Future validation:**

- Sensor fusion under controlled fog / low-visibility conditions.
- Detection performance against manually verified ground truth.
- Field validation on selected HEMM / dumper routes.
- Sensor-failure and degraded-mode testing.

No sensor should be described as fully field-validated until the corresponding hardware and measurement results are demonstrated.

### Source

VISTAX project website:

https://bug-busters-hazel.vercel.app/

---

## 6.2 Driver / Operator

### Expected impact

- Fused sensor information to supplement human visual awareness.
- Real-time advisory warnings for detected hazards / collision-risk situations.
- Earlier warning when direct visibility is degraded.
- Reduced dependence on visual detection alone.
- Driver-assistance support while the operator remains responsible for vehicle control.

### Safety posture

VISTAX is an **advisory driver-assistance system**, not an autonomous vehicle-control system.

The intended VISTAX architecture does not replace the operator's responsibility for vehicle control.

The system should not be represented as automatically controlling steering, braking or vehicle propulsion unless a future certified control architecture is separately implemented and validated.

### Source

VISTAX project website:

https://bug-busters-hazel.vercel.app/

---

## 6.3 Mine Operations

### Expected impact

- Improved visibility into low-visibility operational events.
- Incident and event logging for operational review.
- Near-miss and obstruction records for root-cause analysis.
- Fleet-level analytics for utilization and downtime patterns.
- Centralized vehicle, alert and sensor-health information.
- Decision support for low-visibility operating conditions.
- Potential reduction in avoidable low-visibility interruption time, subject to pilot validation.

### Important limitation

VISTAX should not claim that all mine downtime, production loss or maintenance cost is caused by low visibility.

The operational impact model should isolate low-visibility-related events from unrelated causes such as planned maintenance, industrial relations, equipment breakdown unrelated to visibility, production scheduling, railway constraints or other operational conditions.

---

## 7. Pilot Validation Framework

A field pilot is required before presenting VISTAX performance as a measured industrial result.

### Recommended pilot structure

**Phase 1 — Baseline**

Collect a 30-60 day baseline before VISTAX intervention.

Record:

- Operating hours.
- Visibility conditions.
- Vehicle type.
- Route.
- Haul cycle time.
- Low-visibility interruptions.
- Idle minutes.
- Near-miss / collision-risk events.
- Fuel cost per tonne.
- Unscheduled repair cost.
- Tyre incidents.
- Tonnes moved per operating hour.

**Phase 2 — Controlled VISTAX pilot**

Deploy VISTAX to a selected subset of high-risk routes and selected HEMM / dumpers.

Where practical, use the same:

- Vehicle classes.
- Routes.
- Operating shifts.
- Production context.

The purpose is to compare baseline conditions with VISTAX-assisted operation while controlling for major external factors.

**Phase 3 — Analysis**

Compare:

`Baseline KPI → VISTAX KPI → Normalized change`

Normalize operational measurements where practical for:

- Tonnes moved.
- Operating hours.
- Vehicle class.
- Route.
- Visibility condition.
- Fleet availability.

---

## 8. Pilot KPIs — What Must Be Measured

The following are validation KPIs and must not be represented as already-achieved results.

| KPI | Measurement method | Status |
|---|---|---|
| Detection recall / accuracy | Compare system detections with manually verified ground truth | Pilot validation |
| False-alert rate | False alerts per operating hour / vehicle | Pilot validation |
| Alert latency | Sensor event to driver-alert time | Pilot validation |
| Detection distance | Verified detection distance by scenario | Pilot validation |
| Sensor availability | Percentage of time critical sensors are healthy | Pilot validation |
| Haul cycle time | Baseline vs VISTAX-assisted operation | Pilot validation |
| Low-visibility interruption time | Stopped / interrupted minutes attributable to low visibility | Pilot validation |
| Vehicle idle time | Baseline vs pilot | Pilot validation |
| Fleet utilization | Productive operating time / available time | Pilot validation |
| Operator acceptance | Structured operator feedback | Pilot validation |
| Near-miss events | Events per 1,000 operating hours / trips | Pilot validation |
| Fuel cost per tonne | Fuel cost normalized by tonnes moved | Pilot validation |
| Unscheduled repair cost/hour | Avoidable repair cost per operating hour | Pilot validation |
| Tonnes moved/hour | Baseline vs pilot | Pilot validation |
| Sellable tonnes/dispatched tonnes | Baseline vs pilot | Pilot validation |

### Detection metric definition

A detection target must use a clearly defined metric.

For example:

> **Pilot target: 70–80% recall on the defined controlled test scenarios.**

The final metric definition should specify:

- Object / event classes.
- Distance range.
- Visibility conditions.
- Static vs moving objects.
- Ground-truth method.
- Minimum sample size.
- False-positive measurement method.

The term "detection reliability" should not be used without defining how it is calculated.

---

## 9. Financial Impact Model

The financial model is intentionally separated into two categories:

1. **Cost-saving sensitivity**
2. **Gross revenue-value sensitivity**

These are not equivalent to profit.

### 9.1 Cost-saving sensitivity

NMDC FY 2024-25 company-level reference pool:

`₹210.09 Cr + ₹254.65 Cr = ₹464.74 Cr/year`

Simple monthly equivalent:

`₹464.74 Cr / 12 = ₹38.73 Cr/month`

Illustrative sensitivity:

| Assumed reduction in reference pool | Mathematical value |
|---:|---:|
| 3% | ₹1.16 Cr/month |
| 5% | ₹1.94 Cr/month |

Therefore:

> **Illustrative reference-pool sensitivity: ₹1.2–₹1.9 Cr/month**

This figure is **not a Bailadila-only saving** and is **not an observed VISTAX result**.

A final mine-level saving must use BIOM Bacheli / BIOM Kirandul project-level cost-centre data.

---

## 10. Revenue-Value Sensitivity

NMDC FY 2024-25 reported:

`44.40 MT iron-ore sales`

for:

`₹22,803.40 crore`

This implies a company-wide average realization proxy of approximately:

`₹22,803.40 Cr / 44.40 MT ≈ ₹5,136/tonne`

This is a **NMDC-wide average realization proxy**, not a Bailadila-specific selling price.

### Bailadila / Chhattisgarh sales basis

FY 2024-25:

`30.81 MT/year`

Simple monthly equivalent:

`30.81 / 12 ≈ 2.568 MT/month`

### Illustrative incremental sellable-volume sensitivity

| Incremental sellable tonnage | Approx. monthly tonnage | Gross revenue value at ₹5,136/t |
|---:|---:|---:|
| 0.5% | 12,840 t | ₹6.6 Cr |
| 1.0% | 25,680 t | ₹13.2 Cr |
| 2.0% | 51,360 t | ₹26.4 Cr |

These are **scenario calculations**, not VISTAX performance claims.

The additional tonnes must actually be:

1. Produced.
2. Evacuated.
3. Processed where required.
4. Saleable.
5. Sold.

The calculation also does not deduct incremental mining, crushing, screening, haulage, railway, handling, royalty, statutory or other variable costs.

Therefore:

> **Gross revenue value is not the same as incremental profit.**

---

## 11. Why Cost Saving and Revenue Value Must Be Kept Separate

A single headline number can create a misleading impression when it combines different denominators and assumptions.

The cost-saving sensitivity is based on an **NMDC-wide company-level reference pool**.

The revenue-value sensitivity uses **Bailadila / Chhattisgarh sales volume** multiplied by a **NMDC-wide realization proxy**.

Because these are not both site-level audited values, the following number:

`₹7.8–₹15.1 Cr/month`

must be treated only as a mathematical combination of two independent scenario ranges.

It must **not** be described as:

- Actual VISTAX financial impact.
- Actual Bailadila savings.
- Actual VISTAX profit.
- Guaranteed monthly revenue.
- Guaranteed monthly production benefit.
- Audited ROI.

### Recommended presentation wording

Use:

> **Financial Impact — Modelled Scenario**
>
> Cost-saving sensitivity: ₹1.2–₹1.9 Cr/month*
>
> Gross revenue-value sensitivity: ₹6.6–₹13.2 Cr/month*
>
> `*Derived from FY25 NMDC disclosed reference values and scenario assumptions. Not historical VISTAX performance.`

This is preferable to presenting a single large "profit" number.

---

## 12. Claims That Must Not Be Presented as Actual Results

Do not present the following as proven VISTAX outcomes unless supported by signed-off mine pilot data:

- "Accident reduction of X%."
- "₹X crore/month actual savings."
- "₹X crore/month actual profit."
- "Continuous operation during all fog / monsoon conditions."
- "Zero accidents."
- "Guaranteed production increase."
- "Guaranteed downtime reduction."
- "100% detection."
- "100% sensor availability."
- "Autonomous driving."
- "Complete replacement of NMDC FMS."

Use terminology such as:

- Expected impact.
- Modelled opportunity.
- Pilot target.
- Engineering hypothesis.
- To be validated in field trial.
- Baseline vs pilot measurement.
- Scenario sensitivity.
- Gross revenue value.
- Reference cost pool.

---

## 13. Recommended Bailadila Deployment Plan

### Phase 1 — 90-day pilot

Deploy VISTAX on a controlled subset of high-risk haulage routes and selected HEMM / dumpers at BIOM Bacheli and/or BIOM Kirandul.

Integrate the system with the existing FMS rather than replacing it.

### VISTAX focus areas

1. Low-visibility perception.
2. Forward hazard detection.
3. Collision-risk awareness.
4. Multi-sensor ranging / perception.
5. Local/offline vehicle-side warnings.
6. Event logging for near-miss, obstruction and visibility incidents.
7. Sensor-health monitoring.
8. Linking safety events with fleet and operational KPIs.

### Integration principle

Existing NMDC FMS:

> Fleet management + route + vehicle + operational monitoring

VISTAX:

> Low-visibility perception + hazard awareness + advisory warning + event intelligence

Combined architecture:

> **Existing FMS + VISTAX safety layer**

---

## 14. Post-Pilot Financial Calculation

The final business case should use mine-specific cost-centre and operational data.

### Fuel saving

`Fuel saving = normalized baseline fuel cost − normalized post-pilot fuel cost`

Fuel costs should be normalized for tonnes moved, operating hours and relevant fleet / route conditions.

### Repair saving

`Repair saving = baseline avoidable repair cost − post-pilot avoidable repair cost`

Only repairs causally related to the evaluated operating condition should be included.

### Downtime value

`Downtime value = verified recovered operating hours × verified contribution per operating hour`

### Revenue value

`Gross revenue value = incremental sellable tonnes × realized price per tonne`

### Contribution value

`Incremental contribution = incremental sellable tonnes × contribution margin per tonne`

### Net financial benefit

`Net benefit = verified cost savings + incremental contribution − VISTAX operating cost`

### ROI

`ROI = annual net benefit / VISTAX investment cost`

### Payback period

`Payback period = VISTAX deployment cost / verified monthly net benefit`

A final ROI or payback period should only be stated after site-level pilot measurements and deployment-cost data are available.

---

## 15. Key Facts for Presentation

Use the following as the factual baseline:

> **Bailadila / Chhattisgarh FY25:** 29.98 MT production and 30.81 MT sales.

> **NMDC FY25:** 44.07 MT iron-ore production and 44.40 MT iron-ore sales.

> **NMDC FY25 iron-ore sales value:** ₹22,803.40 crore, implying approximately ₹5,136/t average company-wide realization.

> **NMDC FY25 reference cost pool:** ₹210.09 crore for petrol/diesel/LDO/lubricants and ₹254.65 crore for repairs & maintenance.

> **NMDC FY25 safety reference:** 0 worker fatalities reported at company level and worker LTIFR of 0.17.

> **Historical operational context:** a 40-day FY24-25 Bailadila production stoppage was reported due to Industrial Relations, not low visibility.

> **Digital baseline:** NMDC already has Fleet Management System capabilities at Bailadila and reports vision-enhancement initiatives for dumper movement during foggy weather.

> **VISTAX positioning:** augmentation of the existing digital ecosystem with low-visibility perception, collision-risk awareness, advisory driver assistance and safety-event intelligence.

---

## 16. Source Interpretation Rules

The following terminology should be used consistently throughout the VISTAX project:

### Actual / Disclosed

A value explicitly reported by NMDC or a Government source.

### Calculated

A mathematical result derived directly from disclosed values.

Example:

`₹22,803.40 Cr / 44.40 MT ≈ ₹5,136/t`

### Modelled

A planning assumption applied to a disclosed baseline.

Example:

`3% × ₹38.73 Cr/month = ₹1.16 Cr/month`

### Target

A desired or proposed pilot-performance threshold.

Example:

`70–80% recall target`

### Expected impact

An engineering hypothesis that requires field validation.

### Pilot result

A measured result obtained from a defined field or controlled test and supported by documented test data.

---

## 17. Primary References

### Government / PSU sources

1. **NMDC Limited — Annual Report 2024-25**  
   Production, sales, financials, safety, FMS, digital initiatives and operations.  
   https://www.nmdc.co.in/cms-admin/Upload/Annual_Report_Documents/38e8511b260c46fe9ab44c1948362166_20250807000209693.pdf

2. **NMDC Limited — Production & Sales of Iron Ore, March 2025 disclosure**  
   FY25 Chhattisgarh / Bailadila and company production and sales.  
   https://www.nmdc.co.in/cms-admin/Upload/Production_Sales_Prices_Documents/5769694fba1c42aaabf5b02afc78bad6_20250401155049736.pdf

3. **Ministry of Steel — Annual Report 2024-25**  
   NMDC Fleet Management System and digitalization references.  
   https://steel.gov.in/sites/default/files/2025-04/Steel_English_AR_2024%20%281%29.pdf

4. **NMDC — Sustainability / BRSR FY 2024-25**  
   Fuel-consumption and sustainability data.  
   https://www.nmdc.co.in/cms-admin/Upload/Environment_Sustainability_Documents/18ffd21ac9fa4c71a9578eb82909d301_20260131151221344.pdf

5. **Government of India Forest / FAC record**  
   Bailadila FY24-25 production and 40-day IR-related stoppage.  
   https://forestsclearance.nic.in/writereaddata/FAC_Minutes/6119121212151document%2824%29.pdf

6. **Smart India Hackathon 2026 — Problem Statement Portal**  
   SIH26007 problem context.  
   https://www.sih.gov.in/sih2026PS

### Project source

7. **VISTAX — Mine Vehicle Safety, SIH 2026 PS 26007**  
   Current project architecture and prototype scope.  
   https://bug-busters-hazel.vercel.app/

---

## 18. Recommended Website Report Label

Use:

> **TECHNICAL IMPACT REPORT**  
> Bailadila, NMDC — Evidence, Financial Model & Validation Plan

Recommended note:

> **Data basis:** NMDC FY2024-25 disclosures, Government of India / Ministry of Steel references, and the VISTAX project architecture. Projected values are planning estimates, scenario calculations or pilot targets, not historical VISTAX savings.

---
