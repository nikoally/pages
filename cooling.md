---
layout: page
title: Industrial Cooling
permalink: itac-training/cooling/
---

## Introduction
Cooling systems are essential in industrial facilities to regulate temperature, ensure equipment longevity, and maintain product quality. Two primary cooling technologies used in industrial settings are **chillers** and **cooling towers**. This module explores their operation, energy efficiency considerations, and best practices for optimization.

## Chillers

![Chiller](/assets/chiller.jpg)

Chillers are refrigeration systems that remove heat from a process fluid or space. They operate using either a **vapor compression cycle** or an **absorption refrigeration cycle**.

### Types of Chillers
1. **Air-Cooled Chillers**
   - Use ambient air to remove heat from the refrigerant
   - Suitable for facilities with limited water availability
   - Higher energy consumption compared to water-cooled chillers
   
2. **Water-Cooled Chillers**
   - Use water from a cooling tower to dissipate heat
   - More efficient in large-scale applications
   - Require additional maintenance due to water treatment needs

3. **Absorption Chillers**
   - Use heat instead of electricity to drive the cooling cycle
   - Often powered by waste heat or steam from industrial processes
   - Lower electrical consumption but higher capital costs

### Chiller Efficiency Metrics
- **Coefficient of Performance (COP)**: Ratio of cooling output to energy input
- **Integrated Part Load Value (IPLV)**: Measures efficiency under varying load conditions
- **Kilowatts per Ton (kW/ton)**: Power required to produce one ton of cooling

### Optimization Strategies
- **Proper sizing**: Avoid oversizing, which leads to inefficiencies
- **Variable speed drives (VSDs)**: Adjust compressor speed based on cooling demand
- **Regular maintenance**: Clean heat exchangers, check refrigerant levels, and inspect insulation
- **Load shifting**: Use thermal energy storage to shift cooling loads to off-peak hours

### More Resources

Check out this video by Mike Muller going in-depth about chillers:

{% include youtube.html id="MIptjpNytso" %}

Check out this video about how chillers operate: 

{% include youtube.html id="gYcNDT1d30k" %}

## Cooling Towers

![Cooling Tower](/assets/cooling-tower.jpg)

Cooling towers remove heat from water-cooled systems by evaporating water into the atmosphere. They are widely used in conjunction with water-cooled chillers to enhance efficiency.

Check out this video discussing how they work on a high-level: 

{% include youtube.html id="sWJCWDpY9is" %}

### Types of Cooling Towers
1. **Open-Circuit (Wet) Cooling Towers**
   - Water directly contacts air, allowing heat dissipation through evaporation
   - Highly efficient but requires water treatment to prevent scaling and biological growth

2. **Closed-Circuit (Dry) Cooling Towers**
   - Use a heat exchanger to separate process water from cooling air
   - Lower water consumption but less efficient than open-circuit towers

### Key Performance Indicators
- **Approach Temperature**: Difference between cooled water temperature and ambient wet-bulb temperature
- **Cycles of Concentration (COC)**: Ratio of dissolved solids in recirculating water to makeup water
- **Drift Loss**: Water loss due to fine droplets escaping with exhaust air

### Optimization Strategies
- **Install variable frequency drives (VFDs)**: Adjust fan speeds based on load
- **Monitor water chemistry**: Prevent scaling and biological contamination

### More Resources

Check out this video by Mike Muller discussing cooling towers: 

{% include youtube.html id="4EVJHPnAHEo" %}


## Activity

Objective:

Calculate the energy and demand savings associated with upgrading an older chiller system to a more efficient model using provided efficiency, runtime, and capacity data.

Problem Statement:

A manufacturing plant operates a set of four Carrier chillers, three of which were installed in 1995 and have degraded efficiency. The original efficiency of these older chillers was 0.67 kW/ton, but due to degradation over 29 years, the efficiency has worsened to 0.90 kW/ton. The plant is considering replacing these with modern chillers with an efficiency of 0.60 kW/ton.

Using the following provided data, calculate the annual energy savings (kWh) from upgrading the older chillers.

Given Data:
	- Chiller capacity = 1,250 tons
	- Efficiency of degraded chillers = 0.90 kW/ton
	- Efficiency of new chillers = 0.60 kW/ton
	- Annual runtime of older chillers = 8,760 hours × 54.57% = 4,780.33 hours
	- Degradation factor formula:
\\[\text{Efficiency}_{\text{Degraded}} = \frac{\text{Efficiency}_{\text{Original}}}{(1 - 0.01)^{\text{Age}}}\\]

Tasks:
	1.	Recalculate the degraded efficiency of the older chillers using the formula above, assuming an original efficiency of 0.67 kW/ton and an age of 29 years.
    
	2.	Calculate the annual energy savings in kWh using the formula:
\\[\text{Consumption Savings} = \text{Capacity} \times (\text{Efficiency}{\text{Degraded}} - \text{Efficiency}{\text{New}}) \times \text{Annual Runtime}\\]

{% raw %}
    <h2>Cooling Towers & Chillers Quiz</h2>

    <h3>1. What is the primary function of a cooling tower in an HVAC or industrial system?</h3>
    <input type="radio" name="q1" value="a"> a) Increase air temperature<br>
    <input type="radio" name="q1" value="b"> b) Remove heat from a process by evaporative cooling<br>
    <input type="radio" name="q1" value="c"> c) Generate electricity<br>
    <input type="radio" name="q1" value="d"> d) Convert water into steam<br>

    <h3>2. Which factor has the greatest impact on the efficiency of a cooling tower?</h3>
    <input type="radio" name="q2" value="a"> a) The material of the fill media<br>
    <input type="radio" name="q2" value="b"> b) The relative humidity of the surrounding air<br>
    <input type="radio" name="q2" value="c"> c) The speed of the circulation pump<br>
    <input type="radio" name="q2" value="d"> d) The size of the fan motor<br>

    <h3>3. What is the main difference between an air-cooled chiller and a water-cooled chiller?</h3>
    <input type="radio" name="q3" value="a"> a) Air-cooled chillers use fans to dissipate heat, while water-cooled chillers use cooling towers<br>
    <input type="radio" name="q3" value="b"> b) Air-cooled chillers require less maintenance than water-cooled chillers<br>
    <input type="radio" name="q3" value="c"> c) Water-cooled chillers are only used in industrial applications<br>
    <input type="radio" name="q3" value="d"> d) Air-cooled chillers cannot operate in humid environments<br>

    <h3>4. Which component in a chiller is responsible for compressing the refrigerant and increasing its pressure?</h3>
    <input type="radio" name="q4" value="a"> a) Evaporator<br>
    <input type="radio" name="q4" value="b"> b) Condenser<br>
    <input type="radio" name="q4" value="c"> c) Compressor<br>
    <input type="radio" name="q4" value="d"> d) Expansion valve<br>

    <h3>5. What's the kWh savings from the activity? Round to the nearest kWh. </h3>
    <input type="text" id="q5">


    <br><br>
    <button onclick="checkAnswers()">Submit</button>

    <h3 id="score"></h3>

    <script>
        function checkAnswers() {
            let score = 0;

            // Check Question 1 (Cooling Tower Function)
            let q1Answer = document.querySelector('input[name="q1"]:checked');
            if (q1Answer && q1Answer.value === "b") {
                score += 1;
            }

            // Check Question 2 (Cooling Tower Efficiency)
            let q2Answer = document.querySelector('input[name="q2"]:checked');
            if (q2Answer && q2Answer.value === "b") {
                score += 1;
            }

            // Check Question 3 (Air vs Water Chiller)
            let q3Answer = document.querySelector('input[name="q3"]:checked');
            if (q3Answer && q3Answer.value === "a") {
                score += 1;
            }

            // Check Question 4 (Chiller Compressor)
            let q4Answer = document.querySelector('input[name="q4"]:checked');
            if (q4Answer && q4Answer.value === "c") {
                score += 1;
            }

            // Check Question 5 (Solution)
            let q5Answer = document.getElementById('q5').value.trim();
            if (q5Answer === "1772991") {
                score += 1;
            }

            // Display the score
            document.getElementById('score').innerHTML = "Your score: " + score + "/5";
        }
    </script>

{% endraw %}