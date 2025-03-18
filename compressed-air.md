---
layout: page
title: Compressed Air
permalink: itac-training/compressed-air/
---

## Summary

Compressed air is a crucial, yet costly, resource widely used in manufacturing for powering tools, actuators, and various processes. Although convenient, compressed air typically has efficiency rates of only around 10–15%, making it significantly more expensive than direct electrical power.

Compressed air systems consist of two main areas:

- **Supply Side:** Includes compressors, dryers, filters, and storage tanks.
- **Demand Side:** Includes distribution piping, secondary storage, leaks, and end-use applications.

Improving compressed air efficiency is vital for reducing energy costs, minimizing environmental impact, and achieving sustainability targets.

---

## Supply-Side Energy Saving Measures

### 1. Cold Air Intake

Using colder, denser air for compressor intake reduces the energy required for compression. Cooler air lowers energy consumption and improves the efficiency and lifespan of your compressor.

**Best Practice:**  
Draw compressor intake air from a cooler location (e.g., outside air or air-conditioned spaces) rather than from the hot compressor room.

### 2. Turn Off Compressors When Not in Use

Running compressors unloaded wastes significant energy. Older rotary screw compressors can use up to 85% of their full load power even when idle.

**Best Practice:**  
Use controls or scheduling to ensure compressors are turned off during low demand periods. Consider smaller compressors for low-load conditions.



### 3. Reduce Setpoint Pressure

Compressors often operate at higher pressures than needed. Every unnecessary 2 psi increase in pressure can increase energy use by approximately 1%.

**Best Practice:**  
Regularly measure pressure requirements and lower compressor pressure setpoints to the minimum needed by your facility’s processes.

### 4. Optimize Storage and Distribution

Adequate storage (receiver tanks) and proper piping reduce pressure drops and stabilize system performance. This minimizes the need for extra compressor runtime.

**Best Practice:**  
Design piping with minimal bends and appropriate diameter. Strategically place air receivers near heavy-use areas.

## Demand-Side Energy Saving Measures

### 1. Avoid Using Compressed Air for Personal Cooling

Using compressed air for personal cooling is highly inefficient and wasteful.

**Best Practice:**  
Educate employees about compressed air costs and provide alternative cooling solutions, such as fans.

### 2. Use Engineered Air Nozzles

Open-ended tubes or basic air guns consume excessive air. Engineered air nozzles significantly reduce air consumption and noise levels.

**Best Practice:**  
Replace open-ended hoses and simple nozzles with engineered alternatives designed to maximize efficiency and airflow.

**Diagram Suggestion:**  
- Side-by-side demonstration of airflow and consumption rates of engineered nozzles versus open-ended tubes.

### 3. Detect and Fix Leaks

Leaks typically account for 20–30% of a plant’s total compressed air usage, resulting in considerable waste.

**Best Practice:**  
Conduct routine leak inspections using ultrasonic detection or simple auditory inspections, and promptly repair identified leaks.

### 4. Optimize End-Use Applications

Compressed air is often used where more efficient alternatives exist, such as electric motors or blowers.

**Best Practice:**  
Identify non-essential compressed air uses and replace them with more efficient alternatives.

Examples include:
- Electric blowers instead of compressed air for continuous cleaning.
- Mechanical agitators instead of compressed air for liquid mixing.

---

## Activity

### Scenario Overview

You are conducting an energy assessment at a manufacturing facility. The facility operates daily from **6:00 am to 4:00 pm**, Monday to Friday. However, from **2:00 pm to 4:00 pm**, only the warehouse is active, which does not require compressed air.

### Observations from Site Visit:

- One large air compressor continuously operates at **120 psi**.
- The maximum pressure required by equipment is only **90 psi**.
- The compressor requires 208V
- Compressor intake air is drawn from the hot compressor room (~90°F).
- Audible leaks were identified throughout distribution piping and at an old, unused packaging machine still connected to the system.
- At **6 workstations**, employees regularly use compressed air guns rated at **14 cfm @ 100 psi** to clean workstations. Observations showed each worker used compressed air for **2 minutes per 30 minutes**.
- Previous calculations have established that each **CCF** (100 cubic feet) of compressed air consumes **0.24 kWh**.


### Data Analysis Exercise

You have been provided two weeks of compressor CT (current transducer) data.

#### Task:

Analyze the scenario and calculate the annual energy savings (in kWh) achievable by:

**1. Turning off compressors during non-production warehouse-only hours (2:00 pm–4:00 pm).**  
**2. Eliminating the inappropriate use of compressed air for workstation cleaning.**

[Download Data](assets/data_for_iac_trimmed.csv)

##### Step-by-step Guidance:

- **Production Schedule:**
  - Operating hours: 6:00 am–4:00 pm (10 hours/day).
  - Facility operates 5 days per week, 50 weeks per year.

- **Workstation Cleaning Usage:**
  - Number of workstations: 6
  - Usage per workstation: 2 mins every 30 mins
  - Total daily cleaning time per workstation: 4 mins/hr × 8 production hours (6 am–2 pm) = 32 mins/day/workstation
  - Air nozzle rating: 14 cfm at 100 psi

- **Energy Usage:**
  - Conversion rate: 1 CCF (100 cubic feet) of compressed air = 0.24 kWh

#### Analysis Questions:

1. **Calculate the annual energy savings (in kWh)** from turning compressors off during non-production warehouse-only hours.

2. **Calculate the annual energy savings (in kWh)** from eliminating compressed air workstation cleaning.

3. **Discuss which measure provides greater savings** and whether implementing both measures is beneficial or not. 

---

{% raw %}
<body>
    <h2>Compressed Air Quiz</h2>

    <!-- Question 1: kWh Savings from Shutting Down Compressor -->
    <h3>1. What's the yearly kWh savings for shutting down the compressor? Round to the nearest kWh.</h3>
    <input type="text" id="q1">

    <!-- Question 2: kWh Savings from Stopping Compressed Air for Cleaning -->
    <h3>2. What's the yearly savings for discontinuing the use of compressed air for cleaning? Round to the nearest kWh.</h3>
    <input type="text" id="q2">

    <!-- Question 3: Higher Implementation Cost -->
    <h3>3. Which recommendation is likelier to have a higher implementation cost?</h3>
    <input type="radio" name="q3" value="Shutdown"> Shut Down Compressor<br>
    <input type="radio" name="q3" value="StopUsing"> Stop Using Compressed Air for Cleaning<br>

    <!-- Question 4: Effect of Lowering Setpoint -->
    <h3>4. If the compressor setpoint were lowered from 120 psi to 90 psi, how would this affect each of your recommendations?</h3>
    <input type="radio" name="q4" value="DecreaseBoth"> Decrease savings for both<br>
    <input type="radio" name="q4" value="IncreaseBoth"> Increase savings for both<br>
    <input type="radio" name="q4" value="NoEffect"> No effect on savings<br>
    <input type="radio" name="q4" value="DecreaseShutdownIncreaseCleaning"> Decrease savings for shutting down, increase savings for stopping cleaning<br>

    <!-- Question 5: Most Common Compressor Type -->
    <h3>5. What's the most common type of compressor seen on assessments?</h3>
    <input type="radio" name="q5" value="RotaryScrew"> Rotary Screw<br>
    <input type="radio" name="q5" value="Reciprocating"> Reciprocating<br>
    <input type="radio" name="q5" value="Centrifugal"> Centrifugal<br>
    <input type="radio" name="q5" value="Scroll"> Scroll<br>

    <br><br>
    <button onclick="checkAnswers()">Submit</button>

    <h3 id="score"></h3>

    <script>
        function checkAnswers() {
            let score = 0;

            // Check Question 1 (kWh Savings from Shutting Down Compressor)
            let q1Answer = document.getElementById('q1').value.trim();
            if (q1Answer === "5481") {
                score += 1;
            }

            // Check Question 2 (kWh Savings from Stopping Compressed Air for Cleaning)
            let q2Answer = document.getElementById('q2').value.trim();
            if (q2Answer === "28") {
                score += 1;
            }

            // Check Question 3 (Higher Implementation Cost)
            let q3Answer = document.querySelector('input[name="q3"]:checked');
            if (q3Answer && q3Answer.value === "Shutdown") {
                score += 1;
            }

            // Check Question 4 (Effect of Lowering Setpoint)
            let q4Answer = document.querySelector('input[name="q4"]:checked');
            if (q4Answer && q4Answer.value === "DecreaseBoth") {
                score += 1;
            }

            // Check Question 5 (Most Common Compressor Type)
            let q5Answer = document.querySelector('input[name="q5"]:checked');
            if (q5Answer && q5Answer.value === "RotaryScrew") {
                score += 1;
            }

            // Display the score
            document.getElementById('score').innerHTML = "Your score: " + score + "/5";
        }
    </script>

{% endraw %}