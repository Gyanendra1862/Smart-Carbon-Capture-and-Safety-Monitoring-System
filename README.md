
# 🌳 Smart Urban Tree

### Carbon Capture & Safety Monitoring System

**An integrated smart urban unit concept for particulate air cleaning,
environmental monitoring, and public-safety awareness.**

![Project](https://img.shields.io/badge/Project-Engineering%20Design%20%26%20Fabrication-ff7a00?style=for-the-badge)
![CAD](https://img.shields.io/badge/CAD-SolidWorks-red?style=for-the-badge&logo=dassaultsystemes)
![Platform](https://img.shields.io/badge/Controller-Raspberry%20Pi-c51a4a?style=for-the-badge&logo=raspberrypi)
![Domain](https://img.shields.io/badge/Domain-Smart%20City%20%7C%20IoT-167d9a?style=for-the-badge)
:::

------------------------------------------------------------------------

## 🎬 Project Video & Media

The project video and related media are available in the shared Google Drive folder:

**[▶ Open Smart Urban Tree project video & media folder](https://drive.google.com/drive/folders/1eBxXOKAoQj-OSrxr-slsQ0yJc3F-d2nE)**

> Note: This URL opens a Google Drive folder, not a direct video file. Visitors can open the video from inside the folder. For an embedded video preview on GitHub, add a direct YouTube link or a direct video-file link.

------------------------------------------------------------------------

## 🖼️ CAD Model Gallery

The repository contains SolidWorks part, assembly, and drawing files.
Add screenshots exported from SolidWorks to the `assets/cad/` folder,
then replace the image placeholders below with the exact image
filenames.

Create this folder structure in your repository:

``` text
Smart-Carbon-Capture-and-Safety-Monitoring-System/
├── README.md
├── assets/
│   └── cad/
│       ├── overall-assembly.png
│       ├── front-view.png
│       ├── side-view.png
│       └── exploded-view.png
├── *.SLDPRT
├── *.SLDASM
└── *.SLDDRW
```

  -------------------------------------------------------------------------------------------------------------
  Overall assembly                                             Front view
  ------------------------------------------------------------ ------------------------------------------------
  `![Overall CAD assembly](assets/cad/overall-assembly.png)`   `![Front CAD view](assets/cad/front-view.png)`

  -------------------------------------------------------------------------------------------------------------

  -----------------------------------------------------------------------------------------------------
  Side view                                      Exploded view
  ---------------------------------------------- ------------------------------------------------------
  `![Side CAD view](assets/cad/side-view.png)`   `![Exploded CAD view](assets/cad/exploded-view.png)`

  -----------------------------------------------------------------------------------------------------

> **CAD image note:** These are image-path placeholders, not uploaded
> screenshots. Add your actual SolidWorks screenshots using the
> filenames above (or change the paths to match your filenames).
> Recommended: use a clean isometric view with the model fully visible
> and a plain background.

------------------------------------------------------------------------

## 📌 Project Overview

The **Smart Urban Tree** is a floor-standing smart urban infrastructure
concept that combines an electrostatic-precipitator-based
particulate-removal unit with environmental and public-safety
monitoring. It is intended for high-density public spaces where air
quality and timely awareness of safety events are important.

The concept brings together: - ⚡ ESP-based removal of airborne
particulate matter and smoke. - 🌡️ Temperature and humidity
monitoring. - 🌫️ Air-quality sensing. - 🧠 Raspberry Pi-based monitoring
and automation. - 📟 LCD status display and proposed cloud data
upload. - 🎙️ Audio and vibration-based event monitoring. - 📷
Camera-based recording and alert concept.

> **Technical clarification:** An electrostatic precipitator (ESP)
> removes charged particles such as dust and smoke from an air stream.
> It does not, by itself, capture gaseous carbon dioxide (CO₂). The
> "carbon capture" wording in the project title reflects the supplied
> project title; the documented ESP mechanism is particulate removal.

## 🎯 Objectives

1.  Explore an integrated approach to air-quality improvement and
    public-safety monitoring in crowded urban environments.
2.  Monitor air-quality and environmental conditions.
3.  Detect possible emergency sounds and vibration/tampering events.
4.  Provide local status information and support remote monitoring.
5.  Develop a compact public-facing unit inspired by the form of an
    urban tree.

## ⚙️ System Architecture & Workflow

``` text
          Ambient Air Intake
                  │
                  ▼
       ESP-based Particulate Removal
                  │
                  ▼
             Clean Air Out

  AQI / Temperature / Humidity Sensing
                  │
                  ▼
       Raspberry Pi Control & Automation
                  │
          ┌───────┴────────┐
          ▼                ▼
    LCD Display       Cloud Data Upload
          │
          ▼
 Emergency Detection (Audio + Vibration)
          │
          ▼
  360° Camera Recording + Alerts
          │
          ▼
     ESP Self-Cleaning Concept
```

## ✨ Main Functionalities

  -----------------------------------------------------------------------
  Feature                             Description
  ----------------------------------- -----------------------------------
  🌬️ Particulate cleaning             ESP-based removal of dust, fine
                                      particles, and smoke from the
                                      airflow

  🌡️ Environmental monitoring         Temperature and humidity sensing

  📊 Air-quality monitoring           MQ-135-based air-quality sensing

  🚨 Emergency awareness              Audio and vibration input for
                                      possible emergency/tampering events

  📷 Camera monitoring                Proposed 360° recording and alert
                                      response

  ☁️ IoT monitoring                   Wi-Fi/LAN connectivity and proposed
                                      cloud-data upload

  🔄 Continuous operation concept     ESP self-cleaning mechanism
                                      proposed in the design
  -----------------------------------------------------------------------

## 📐 Technical Specifications

  -----------------------------------------------------------------------
  Parameter                           Design specification
  ----------------------------------- -----------------------------------
  Unit type                           Floor-standing smart urban unit

  Approximate dimensions              120--150 cm (H) × 45--50 cm (W) ×
                                      35--40 cm (D)

  Approximate weight                  18--25 kg

  Enclosure                           Insulated metal--plastic enclosure

  Air-treatment method                Electrostatic precipitator

  Target airflow                      250--400 m³/hr

  Stated removal efficiency           90--95% (design target; requires
                                      experimental validation)

  Input supply                        230 V AC

  Average power consumption           60--90 W

  Operating temperature               0--50 °C

  Operating humidity                  10--90% RH

  Connectivity                        Wi-Fi / LAN

  Backup                              Optional battery / UPS
  -----------------------------------------------------------------------

*Specifications are reproduced from the project design poster and should
be treated as proposed targets unless verified by prototype testing.*

## 🔩 Hardware & Bill of Materials

  ------------------------------------------------------------------------------
                   No. Component                       Qty. Purpose
  -------------------- --------------- -------------------- --------------------
                     1 Raspberry Pi 3                     1 Main controller
                       B+                                   

                     2 32 GB Class-10                     1 Operating system and
                       microSD card                         data storage

                     3 Microphone                         1 Sound/noise input
                       module                               

                     4 DHT11                              1 Temperature and
                                                            humidity sensing

                     5 Relay                              1 Electrical switching

                     6 MQ-135                             1 Air-quality sensing

                     7 Raspberry Pi                       1 Image/video capture
                       camera                               

                     8 16×2 LCD with                      1 Local display
                       driver                               

                     9 Stepper motor                      1 Controlled
                                                            rotational movement

                    10 ULN2003 stepper                    1 Stepper motor
                       motor driver                         control

                    11 Vibration motor                    1 Vibration
                                                            alert/notification

                    12 Electrostatic                      1 Particulate and
                       precipitator                         smoke removal

                    13 5 V DC adapter                     1 Low-voltage power
                                                            supply

                    14 Enclosure                        --- Physical structure
                       material                             

                    15 Wires, PCB and                   --- Electrical
                       connectors                           integration
  ------------------------------------------------------------------------------

**Estimated project cost in the poster: ₹24,200.** Actual cost may vary
with component selection and procurement.

## 🧩 SolidWorks CAD Files

This repository includes mechanical CAD files created using SolidWorks:

-   `.SLDPRT` --- Individual part models.
-   `.SLDASM` --- Mechanical assemblies.
-   `.SLDDRW` --- Engineering drawings.

Open the assembly files in SolidWorks to inspect the mechanical
arrangement. Keep referenced part and assembly files together when
opening the project to avoid missing-reference warnings.

## 🧪 Project Methodology

The project follows a five-step design process:

1.  **Empathize** --- Understand public-space air-quality and safety
    concerns.
2.  **Define** --- Identify the core problem and system requirements.
3.  **Ideate** --- Explore integrated design concepts.
4.  **Prototype** --- Develop the proposed system and CAD design.
5.  **Test** --- Evaluate system operation and refine the design.

## 🛡️ Safety & Validation Notes

-   The ESP section uses high voltage. Insulation, grounding, enclosure,
    electrical isolation, and safe discharge arrangements must be
    designed and checked by qualified personnel.
-   Isolate the power supply and follow a safe discharge procedure
    before servicing the ESP.
-   Protect users from energized components and moving mechanisms.
-   Verify wiring, fusing, power ratings, and enclosure protection
    before operation.
-   Camera use in public areas must comply with applicable privacy and
    data-protection requirements.
-   Sensor readings and emergency detection require calibration and
    testing; they should not be treated as certified life-safety systems
    without appropriate validation.

### Tests needed before claiming performance

-   Particle-removal efficiency and airflow under defined test
    conditions.
-   Air-quality sensor calibration and response.
-   Temperature and humidity measurement accuracy.
-   Emergency-event detection reliability and false-alarm rate.
-   Camera coverage, recording, and alert operation.
-   ESP cleaning effectiveness and electrical safety.
-   Actual power consumption and continuous-operation performance.

## 👥 Project Team

**Course:** DS3001 --- Engineering Design Including Design and
Fabrication\
**Institution:** PDPM IIITDM Jabalpur\
**Mentor:** Dr. Shyam Kumar Chokka

  Team member             Roll number
  ----------------------- -------------
  Chittiki Navya Sri      23BCS070
  C. Bhavya Sri           23BME025
  Gyanendra Kumar         23BSM027
  Kotte Meghana           23BCS139
  Kolla Venkata Pradeep   23BCS136
  Trinetra Sathish        23BDS059

## 📚 References

The project poster lists these references:

1.  https://www.mdpi.com/1424-8220/15/12/31392
2.  https://dergipark.org.tr/en/pub/thermal/article/529054
3.  https://onlinelibrary.wiley.com/doi/full/10.1111/j.1539-6924.2012.01900.x
4.  https://oxfordre.com/communication/display/10.1093/acrefore/9780190228613.001.0001/acrefore-9780190228613-e-145
5.  https://www.taylorfrancis.com/books/mono/10.4324/9781315838779/global-warming-danny-harvey

------------------------------------------------------------------------

<img width="3072" height="4096" alt="IMG20260504150100" src="https://github.com/user-attachments/assets/46eabb8f-5ab2-4be1-a305-528176685d55" />
<img width="519" height="556" alt="Screenshot 2026-03-15 002338" src="https://github.com/user-attachments/assets/2e4d54a2-1b2f-469a-a7d7-69c2830f976c" />

### 🌍 Smart Design • Cleaner Air • Safer Public Spaces

**Engineering Design Including Design and Fabrication --- PDPM IIITDM
Jabalpur**
:::
