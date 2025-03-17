---
layout: page
title: Utility Analysis
permalink: itac-training/utility-analysis/
---

Utility analysis is critical for identifying cost-saving opportunities in manufacturing energy assessments. It involves understanding your energy bills, identifying trends, and pinpointing inefficiencies.

## Types of Energy Bills

Manufacturing firms typically encounter these types of energy bills:

- **Electricity:** Powers machinery, lighting, HVAC, compressed air systems, refrigeration, and office equipment.
- **Natural Gas:** Commonly used for heating, boilers, process heat, ovens, and drying processes.
- **Propane:** Often used for heating, forklifts, portable heaters, or remote equipment in locations without natural gas infrastructure.
- **Fuel Oil:** Used primarily for boilers, heating, backup generators, or industrial furnaces, especially in locations without natural gas access.

---

## Overarching Recommendations

There's a few recommendations that are broadly applicable across many different types of energy bills. 

### 1. **Pay Bills on Time**
- Avoid late fees, which can typically range from 1% to 5% of the total bill.
- **Savings Calculation:**
  \\(
  \text{Annual Savings} = \text{Average monthly late fee} \times 12
  \\)

### 2. **Review and Switch Rate Plans**
- Many utilities offer multiple rate structures such as time-of-use (TOU) or demand-based tariffs.
- Calculate potential savings by comparing your current bill with hypothetical scenarios under alternative rate structures.
- **Savings Calculation:**
  \\(
  \text{Annual Savings} = (\text{Current rate annual cost}) - (\text{Proposed rate annual cost})
  \\)

### 3. **Third-party Energy Suppliers**
- Third-party suppliers might offer competitive energy rates compared to your current utility provider.
- Request quotes from alternative suppliers to compare pricing.
- **Savings Calculation:**
  \\(
  \text{Annual Savings} = (\text{Current annual energy cost}) - (\text{Third-party annual energy cost})
  \\)

### 4. **Tax-free Status**
- Many manufacturing firms are eligible for state tax exemptions on energy use.
- Typically, these taxes range from 3% to 10% of energy costs.
- **Savings Calculation:**
  \\(
  \text{Annual Savings} = (\text{Energy costs}) \times (\text{Tax rate})
  \\)

---

## **Power Factor Correction**

Power factor (PF) measures the efficiency of electricity use, specifically the ratio between real power (used to perform actual work, measured in kilowatts or kW) and apparent power (total power supplied, measured in kilovolt-amperes or kVA). A lower power factor indicates inefficiency, causing utilities to impose penalties (usually below a threshold like 0.90). 

- **Ideal PF:** Typically above 0.90 (or 90%).
- **Poor PF:** Below 0.90 may incur additional charges from utilities due to higher current draw and reduced grid efficiency.

In order to improve power factor, we generally recommend installing power factor correction equipment such as capacitors or capacitor banks, optimizing equipment use, or upgrading inefficient motors.

For a more technical introduciton to power factor, check out this video: 

{% include youtube.html id="Tv_7XWf96gg" %}

## How to Perform Utility Analysis

Effective utility analysis follows these general steps:

1. **Import Data into Excel**
    - Gather 12-24 months of energy bills.
    - Enter bill data into Excel, including:
        - Billing period dates
        - Total consumption (kWh, therms, gallons)
        - Peak demand (kW for electricity)
        - Total costs and any itemized charges (fixed charges, demand charges, etc.)

2. **Calculate Average Rates**
    - Calculate the average electricity rates:
        - Average electricity consumption rate ($/kWh) = total cost ÷ total kWh consumed.
        - Average electricity demand rate ($/kW) = total demand cost ÷ total billed peak demand.
    - For natural gas, propane, and fuel oil:
        - Average cost ($ per therm, gallon, or unit) = total cost ÷ total consumption.

3. **Graph Data and Analyze Trends**
    - Create visualizations, such as monthly consumption, costs, demand, and rate trends.
    - Identify seasonal fluctuations or irregular usage patterns indicating inefficiencies.

4. **Look for Recommendations**
    - Evaluate trends for anomalies, spikes, or inefficiencies.
    - Identify potential cost-saving opportunities, such as the ones mentioned above
  
  ---

## More Information

This video is a part of the IAC 101 series by Mike Muller. It provides more i-depth coverage of the topics discussed here. 

{% include youtube.html id="FShr6CHCmec" %}

In CT, there's a "competitive" electricity market. This effectively means that instead of the governemnt regulating energy prices as closely, they take steps to enable competition for electricity generation. Since electric delivery is a natural monopoly, that is still regulated heavily through government-approved rate tariffs. 

[CT Electricity Rate Board](https://energizect.com/rate-board/compare-energy-supplier-rates)

[Eversource Commercial Rate Tariffs](https://www.eversource.com/content/business/account-billing/manage-bill/about-your-bill/rates-tariffs/electric-tariffs-and-rules)

Also, take a look at this explanation of what different things mean on an Eversource bill. 

[Eversource Understanding Your Bill](https://www.eversource.com/content/business/account-billing/manage-bill/about-your-bill/understanding-your-bill/understanding-supply-and-delivery-charges)

I use eversource here as an example because that's what the majority of our clients use. However, other companies generally have similar versions of these resources if you google hard enough. 

## Activity

Using the data at the link below, conduct a utility analysis (I did step 1 for you). Then, calculate the average kW, kWh, and MMbtu rates. Note that the data provided is in CCF, so you will have to convert units. Finally, identify which recommendations would be relevant for this company and identify the corresponding ARC codes. 


[Download Excel File](assets/utility-analysis-activity.xlsx)

[Download the ARC Manual](https://iac.university/file/technical/ARC%20List%20-%20V21.1.pdf)

## Quiz

{% raw %}

<!-- Question 1: kWh Rate -->
<h4>1. What's the kWh rate for the company in the activity? Provide your answer without the dollar sign and rounded to the nearest cent.</h4>
<input type="text" id="q1">

<!-- Question 2: kW Rate -->
<h4>2. What's the kW rate for the company in the activity?</h4>
<input type="text" id="q2">

<!-- Question 3: High kW Rate -->
<h4>3. What's the main reason the kW rate is so high?</h4>
<input type="radio" name="q3" value="a"> a. They operate in a place where electricity is expensive<br>
<input type="radio" name="q3" value="b"> b. They have a low power factor<br>
<input type="radio" name="q3" value="c"> c. They are on an incorrect rate tariff<br>
<input type="radio" name="q3" value="d"> d. None of the above<br>

<!-- Question 4: ARC Code -->
<h4>4. Which ARC code isn't applicable for the company?</h4>
<input type="radio" name="q4" value="a"> a. 2.3212<br>
<input type="radio" name="q4" value="b"> b. 2.8121<br>
<input type="radio" name="q4" value="c"> c. 2.8123<br>

<br>
<button onclick="checkAnswers()">Submit</button>

<h4 id="score"></h4>

<script>
    function checkAnswers() {
        let score = 0;

        // Check Question 1 (kWh Rate)
        let q1Answer = document.getElementById('q1').value.trim();
        if (q1Answer === "0.11") {
            score += 1;
        }

        // Check Question 2 (kW Rate)
        let q2Answer = document.getElementById('q2').value.trim();
        if (q2Answer === "27.93") {
            score += 1;
        }

        // Check Question 3 (High kW Rate)
        let q3Answer = document.querySelector('input[name="q3"]:checked');
        if (q3Answer && q3Answer.value === "b") {
            score += 1;
        }

        // Check Question 4 (ARC Code)
        let q4Answer = document.querySelector('input[name="q4"]:checked');
        if (q4Answer && q4Answer.value === "c") {
            score += 1;
        }

        // Display the score
        document.getElementById('score').innerHTML = "Your score: " + score + "/4";
    }
</script>
{% endraw %}

