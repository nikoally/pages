---
layout: page
title: HVAC
permalink: itac-training/hvac
---

## Understanding HVAC Systems

HVAC systems regulate temperature, humidity, cleanliness, and air distribution. They significantly impact building energy consumption. Proper design, operation, and maintenance are critical for efficiency and cost-effectiveness.

**Types of Air Conditioning Systems:**
- **Comfort air conditioning:** Controls environment for occupant comfort. This is what you typically think of when you hear "HVAC."
- **Process air conditioning:** Controls air for industrial processes or storage conditions. This can include a variety of things, but the most common is air filtration to reduce the levels of airborne particulates. 

### Major Components

- **Fans**: Move air through the system (centrifugal fans most common).
- **Heating/Cooling Coils**: Transfer heat; efficiency influenced by fins per inch and coil depth.
- **Air Cleaners (Filters)**: Improve indoor air quality and system efficiency.
- **Humidifiers**: Maintain required moisture levels.
- **Control Systems**: Manage temperature, humidity, airflow, and optimize efficiency. You'll often hear these referred to as a "BMS."
- **Air Distribution Systems**: Deliver conditioned air efficiently; poor design results in increased fan horsepower.

Check out this video about how these different components work: 

{% include youtube.html id="UmWWZdJR1hQ" %}


### Psychology
Psychology plays a crucial role in HVAC system design and operation by influencing thermal comfort, user behavior, and energy efficiency. Human perception of temperature, humidity, and airflow varies based on factors like individual preferences, cultural background, and psychological adaptation. HVAC systems must account for these variations to optimize occupant comfort while maintaining energy efficiency. Additionally, behavioral psychology informs how users interact with thermostats and climate controls, impacting overall system performance. By integrating insights from psychology, HVAC designers can develop smarter systems that balance comfort, efficiency, and user satisfaction.

Psychological factors significantly influence how people perceive temperature changes in indoor environments. Studies have shown that if the temperature is subtly decreased by a degree or two over time, most occupants do not notice the difference. However, if they are told that the temperature has changed, regardless of if it was actually changed, many will report feeling too hot or too cold and may even voice complaints. This highlights the power of expectation and perception in thermal comfort. 

From an energy assessment standpoint, occupant behavior can also lead to inefficiencies. When individuals repeatedly adjust thermostats in an attempt to quickly reach their desired temperature—often mashing buttons or setting extreme temperatures—they can cause HVAC systems to cycle inefficiently, leading to unnecessary energy waste. Recognizing this, many advanced commercial thermostats do not immediately adjust the temperature when changed by a user. Instead, they log these adjustments as thermal complaints, allowing facility managers to identify patterns and make strategic adjustments without excessive energy use. This approach helps balance occupant satisfaction with energy efficiency in large-scale HVAC operations.

## Energy Conservation Opportunities

- Operate Systems Only When Necessary:
  - Use scheduling controls; avoid continuous operation.
  - Example: Reducing weekly operation from 168 to 50 hours can save thousands of dollars annually.

- Use outdoor air for cooling when feasible:
  - **Outdoor Temperature Control**: Uses dry-bulb temperature for switching.
  - **Enthalpy Control (Recommended)**: Uses true heat content of air, achieving greater savings.

- Reduce Reheating by avoiding simultaneous heating and cooling, which is inefficient and costly. Aim to:
  - Adjust thermostats to broader ranges (68°F heating, 78°F cooling).
  - Sequence heating and cooling operations to avoid conflicts.

- Reduce Makeup Air. Excessive outdoor air increases heating and cooling loads:
  - Evaluate ventilation requirements critically.
  - Improve sealing and damper controls.
  - IPB switched to 100% makeup air during COVID and still hasn't switched back to a sensible amount. 


## Energy Efficiency Opportunities

When assessing a HVAC system, a lot of the recommendations can overlap with previous topics we've discussed, like motors, chillers, and boilers. However, there's also a few recommendations that are unique to HVAC systems. They generally fall into 3 categories: HVAC control, operation, and RTUs. 

By number of recommendations, HVAC control takes the cake. Here, we have things like: 
- Reduce setpoint during winter/raise it during summer
- Adjust setpoint when no one's in the building
- Install smart thermostats
- Install a BMS
- Avoid introducing hot air into AC system

There's also a few for operations: 
- Condition only the smallest space necessary
- Close doors to conditioned spaces
- Reschedule multiple-source heating systems

And a few about RTUs: 
- Replace aging RTUs
- Use properly sized equipment

## More Resources

A lot of these HVAC recommendations need to be simulated as there aren't easy equations we can apply. The most common software for doing this is EnergyPlus. While learning the software is beyond the scope for now, this is an excellent playlist for learning later on. 

[EnergyPlus Playlist](https://www.youtube.com/playlist?list=PLt8euQ9WuNBcGVJrrWRqlAGmE7HnoQXHc)


## Activity

GreenTech is a mid-sized office building (50,000 sq. ft.) located in a temperate climate zone. The building operates from 7:00 AM to 7:00 PM on weekdays and is unoccupied on weekends. They focus on fonal assembly of electronic devices. There are no PPE requirements.The following observations were noted: 

- All thermostats are old and have no scheduling ability. There are 8 total thermostats in the facility. 
- Temperature setpoint is 72ºF year-round, 24/7. 
- They have air conditioning units installed. They only operate during the summer months. 
- Production levels are constant year-round
- Natural gas is almost exclusively used for heating. 

An energy assessment team recently conducted an audit and identified multiple HVAC inefficiencies. Two key recommendations were:
1.	Install smart thermostats to better control setpoints.
2.	Adjust setpoint temperature at night to 65ºF in the winter and 78ºF in the summer. 


For part 1, use the CT program savings document and the dataset provided below. For part 2, search for a methodology to use and be prepared to defend your choice.  

To determine the kWH used for AC, look at the difference in usage between the cooling months (highlighted) and the heating months. I'd recommend computing the difference between the monthly kWh usage for each cooling months and the average heating month. You can use the same procedure for natural gas, but flipped. 


[CT Program Savings Document](https://energizect.com/sites/default/files/documents/Final2023CTProgramSavingsDocument_030123.pdf)

[Site Data](assets/HVAC-activity.xlsx)


