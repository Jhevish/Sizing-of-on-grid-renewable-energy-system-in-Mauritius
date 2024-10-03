#This is one of my favourite project which i did when I was in my last year of my BEng (Hons) Electrical and Electronic Engineering

# Overview
A specific location is picked, one that is located at L'aventure in the Flacq district and has coordinates of -20.153786° and 057.678401°. In order to determine a system, the load variations and energy consumption are quoted from the proper sources and extrapolated to forecast future demand. A site assessment will provide information on environmental conditions such as temperature, solar energy, wind speed, and other factors. Through that , the selected system has been modelled and simulated using the NREL System Advisor Model (SAM). To determine the most feasible solution, the findings are analyzed, and performance and financial assessment are examined.

#Introduction
# Sizing-of-on-grid-renewable-energy-system-in-Mauritius
Mauritius has no known coal reserves or oil and is therefore heavily dependent on imported energy resources. The electricity production is characterized by the Central Electricity Board (CEB) and the various Independent Power Producers (IPPs). However, environmental issues have been brought to the surface in relation to the energy policy mainly as a result of global warming, caused by emission of greenhouse gases (UNDP, 2022). Mauritius is situated in the tropics as such benefits from 2900 hours of sunlight per annum. In order to encourage the use of solar energy whether for water heating or electricity production, incentive schemes are devised so as to enable long-term goals to be achieved, addressed by the Renewable Energy Masterplan. CEB provides many schemes such as Net-Metering, Gross-Metering and NetBilling to attract interested parties to adopt energy production from renewable resources. Hence, it is worthwhile to investigate the implementation of a grid-tied PV system under proposed schemes for an entity (Green Growth Knowledge Platform, 2022).
The national and international economies were impacted by the COVID-19 pandemic in 2020. Global lockdowns predicted delays in project completion and disruptions in the human capital transfer, supply networks, and market for RE technologies. The pandemic's effects were felt in Mauritius and had a corresponding impact on how RE initiatives were carried out.
The Ministry of Energy and Public Utilities published the Renewable Energy (RE) Roadmap 2030 for the Electricity Sector in 2019 and details how to meet the RE targets of 35% by 2025. To accomplish the goal of 40% RE by 2030, the RE Roadmap took into account the necessary technological investments and included energy options. In contrast to the projected RE objective of 25.2% by 2020, this resulted in an integration of RE of 23.9% in the energy mix.
The Government of Mauritius declared green energy as a new economic pillar of Mauritius in the Budget Speech for 2021/22. The declaration of the phase-out of coal in the production of electricity within the same timeframe coincided with the rise in the RE target in the energy mix from 40% to 60% by 2030. The declaration was issued well in advance of COP26, which will take place in Glasgow in November 2021.

# Site assessment
The co-ordinates were plotted on google maps and a point at the centre was taken as a reference. The site location is at the co-ordinates -20.153786° and 057.678401° and is situated at L’aventure in Flacq. It can be noted that the site is very close to a residential area which thereby makes it not feasible for wind turbines. The site features a perimeter of around 2500m and area about 318000 m2. Land slope at the location is 2 degrees.

![image](https://github.com/user-attachments/assets/58b043ec-3158-4113-93d2-260cd81c1414)

# Data collection
Solar energy is the primary energy source for PV systems. The amount of solar power reaching the Earth’s upper atmosphere is measured by solar irradiance. However, absorption and scattering reduce the power reaching the Earth’s surface. The Global Horizontal Irradiance (kW/m2) is the total irradiance received per unit area on the Earth’s surface. Global Horizontal Insolation defines the amount of solar energy received per unit area on the Earth surface. It differs depending on location, season, and other environmental factors. The table below accounts for the GHI values extracted from PV-GIS. (JRC Photovoltaic Geographical Information System (PVGIS) – European Commission, 2022)

### GHI (kWh/m²)

| Month      | 2017   | 2018   | 2019   | 2020   |
|------------|--------|--------|--------|--------|
| January    | 221.93 | 164.72 | 193.15 | 164.82 |
| February   | 160.63 | 158.57 | 172.72 | 182.92 |
| March      | 168.32 | 151.32 | 174.39 | 132.98 |
| April      | 129.62 | 129.87 | 128.36 | 130.47 |
| May        | 106.05 | 124.44 | 109.42 | 120.50 |
| June       | 104.54 | 103.85 |  96.80 |  97.26 |
| July       | 106.37 | 110.44 | 104.80 | 104.60 |
| August     | 131.30 | 135.33 | 127.65 | 129.47 |
| September  | 152.09 | 152.16 | 144.99 | 148.83 |
| October    | 186.92 | 170.01 | 175.64 | 183.48 |
| November   | 168.04 | 183.44 | 174.39 | 173.73 |
| December   | 216.16 | 193.57 | 191.12 | 185.70 |
| **Yearly** | 1851.97| 1777.72| 1793.43| 1754.76|

*Table 1: GHI variations*

The GHI is the sum of the DNI and DHI. As per the table, lowest GHI values are recorded in winter months such as June and the maximum values are recorded in January and December. This is because the amount of irradiance received on Earth surface during summer periods is larger than during winter periods due to lower cloud coverage and interference.

#Temperature
The temperature has an effect on solar energy production. The efficiency of the PV tends to decrease with increasing temperature, so the design must be able to account for this. To reduce the impact of temperature on energy production, a PV with a low temperature coefficient is preferred. The trend of average temperatures over the last five years for the chosen entity obtained from PV-GIS is tabulated below. The extraction file is found in the appendix. (JRC Photovoltaic Geographical Information System (PVGIS) – European Commission, 2022)

### Temperature (°C)

| Month      | 2017  | 2018  | 2019  | 2020  |
|------------|-------|-------|-------|-------|
| January    | 25.9  | 25.2  | 25.9  | 25.1  |
| February   | 25.4  | 25.3  | 25.6  | 25.3  |
| March      | 25.4  | 25.1  | 26.0  | 25.1  |
| April      | 24.4  | 24.1  | 24.9  | 22.8  |
| May        | 22.7  | 22.8  | 23.0  | 22.5  |
| June       | 21.6  | 21.5  | 21.3  | 20.7  |
| July       | 21.0  | 20.1  | 20.9  | 20.2  |
| August     | 20.5  | 20.9  | 20.7  | 19.9  |
| September  | 21.2  | 21.3  | 21.1  | 20.5  |
| October    | 22.7  | 22.1  | 22.8  | 22.5  |
| November   | 23.5  | 23.9  | 24.2  | 22.8  |
| December   | 25.2  | 25.0  | 25.6  | 23.8  |

*Table 2: Temperature variations*

#Wind Speed
Wind speed is another important factor to consider when designing a PV system. Higher wind speeds tend to remove heat from the surface of the cells, increasing module efficiency. A high wind speed, on the other hand, produces uplift forces that can damage the system's mounting structures. As a result, when designing the system, the wind speeds at the entity must be properly assessed. The monthly wind speed variation for the year 2020 is shown in the table below.

### Wind Speed (m/s) - 2020

| Month      | Wind Speed (m/s) |
|------------|------------------|
| January    | 1.77             |
| February   | 5.65             |
| March      | 4.88             |
| April      | 7.45             |
| May        | 6.55             |
| June       | 8.78             |
| July       | 8.00             |
| August     | 6.86             |
| September  | 6.26             |
| October    | 5.35             |
| November   | 5.30             |
| December   | 7.14             |

*Table 3: Monthly Wind Speed Variations for 2020 (MERRA - www.soda-pro.com, n.d.).*

![image](https://github.com/user-attachments/assets/2d9dea72-1962-4c73-814b-ab074e33a561)


Fig 2: Wind Speed Variations

From the graph we can deduce that the minimum wind speed occurs during the month of January and maximum wind speed during the month of June.

#Clean Energy System (CES)

Based on the location of the site and the available renewable energy resources, although the wind is favorable for setting wind harnessing technologies such as the wind turbine, the social conditions pose to be a hurdle based on the turbine’s noise effect and height. However, solar power can be harnessed since throughout the year, and the GHI values prove that it will be more efficient.

#PV SYSTEM DESIGN

The total GHI obtained each year was 1754.76 kWh/m2 on average. As illustrated below, it is possible to determine the peak sun hours (PSH). The most important figure to calculate for the potential site is the Peak Sun Hours (PSH) per day. This is not a simple measure of daylight hours but rather the equivalent number hours of an amount of standardized solar radiation (1 kW/m2). In the graph below, the red line shows the amount of solar radiation received during a day. The blue line show the equivalent number of PSH. The area under both curves is the same, but since PSH is in standardized units (the same standards that solar panel manufacturers use to rate their panels) this number can be used to choose a solar panel appropriate to the application.



![image](https://github.com/user-attachments/assets/80dca9d0-3aac-43ef-87de-e877660889fc)


Fig 3: PSH calculation (Sizing Solar Power for Off-grid Field Studies, 2022)

For Yearly PSH:

PSH = (Sum of GHI monthly) / 1000 W/m²


#Design specifications for grid-tied PV systems

The proposed systems must meet all the requirements below to be classified as eligible.

### Sizing Requirement 1:

The open circuit voltage \( V_{oc} \) of the array should not exceed the inverter's highest input voltage:

\[
V_{oc \, Array \, max} \leq V_{inv \, max}
\]

The maximum number of modules connected in series, \( N_{s \, max} \), can be found as:

\[
N_{s \, max} = \frac{V_{in \, max}}{V_{oc \, max}}
\]

Where:

\[
V_{oc \, max} = V_{oc} \left( 1 + \beta \left( T_{min} - T_{STC} \right) \right)
\]

So, the number of series modules becomes:

\[
N_{s \, max} \leq \frac{V_{in \, max}}{V_{oc \, max}}
\]

### Where:

- \( V_{in \, max} \): Maximum DC input voltage of the inverter.
- \( V_{oc} \): Open Circuit Voltage at Standard Test Conditions (STC).
- \( V_{oc \, max} \): Maximum open circuit voltage of the module in cold temperature.
- \( \beta \): Temperature coefficient of open circuit voltage.
- \( T_{min} \): Minimum ambient temperature.
- \( T_{STC} \): Temperature at Standard Test Conditions.

### Sizing Requirement 2:

The array minimum voltage should not drop below the inverter’s DC input voltage due to degradation in hot temperatures:

\[
V_{oc \, Array \, min} > V_{inv \, min}
\]

The **minimum** power point voltage \( V_{mpp \, min} \) can be calculated using the formula:

\[
V_{mpp \, min} = V_{m} \left( 1 + \beta \left( T_{max} + T_{adder} - T_{STC} \right) \right)
\]

Where:
- \( V_{mpp \, min} \): Module Maximum Power Point (MPP) voltage at high temperatures.
- \( V_{m} \): Module MPP voltage at Standard Test Conditions (STC).
- \( \beta \): Temperature coefficient of open circuit voltage.
- \( T_{max} \): Maximum ambient temperature on-site.
- \( T_{adder} \): Temperature adder (25°C).
- \( T_{STC} \): Temperature at Standard Test Conditions.

The **minimum** number of modules \( N_{s \, min} \) connected in series is given by:

\[
N_{s \, min} \geq \frac{V_{inv \, min}}{V_{mpp \, min}}
\]

Where:
- \( N_{s \, min} \): Minimum number of modules in series.
- \( V_{inv \, min} \): Minimum DC input voltage of the inverter.

### Sizing Requirement 3:

The maximum short circuit current \( I_{sc-array-max} \) should not exceed the inverter maximum input current \( I_{inv-max} \).

\[
I_{sc-array-max} < I_{inv-max}
\]

\[
I_{sc-string-max} = I_m \times \left( \frac{S}{S_{stc}} \right) \times \left( 1 + T_{\alpha} \left( T_{max} + T_{adder} - T_{stc} \right) \right)
\]

The number of strings in parallel \( N_p \) is given by:

\[
N_p \leq \frac{I_{inv-max}}{I_m \times \left( \frac{S}{S_{stc}} \right) \times \left( 1 + T_{\alpha} \left( T_{max} + T_{adder} - T_{stc} \right) \right)}
\]


#### Definitions:
- \( I_{sc-string-max} \): Maximum short circuit current of the string. The string current is the same as the maximum module short circuit current due to the series connection in the string.
- \( S \): Maximum irradiance at the site of the chosen entity.
- \( S_{stc} \): Irradiance at standard test conditions.
- \( I_m \): Module current at standard test conditions.
- \( T_{\alpha} \): Temperature coefficient of short circuit current.


### Sizing Requirement 4:

The number of parallel strings to be connected can be found by considering the maximum input DC power of the inverter and the total DC power of the string array.

\[
P_{dc (array max)} \leq P_{dc (inv max)}
\]

\[
P_{dc string max} = P_m N_p \left( \frac{S_{max}}{S_{STC}} \right) \times \left( 1 + \gamma \left( T_{max} + T_{adder} - T_{STC} \right) \right)
\]

\[
N_p \leq \frac{P_{inv max}}{P_{string max}}
\]

#### Definitions:
- \( P_m \): Maximum power of module at STC.
- \( \gamma \): Temperature coefficient of power.
- \( P_{dc string max} \): DC power through each string.

---

Different systems were designed, taking into consideration cost, efficiency, and space availability, and the most appropriate one was chosen. Two weather files were extracted and chosen from SAM software: year 2018 and 2019. The 2018 one was chosen for system design 1 and 2, and the remaining designs catered for 2019. Since the allowable power range is below 15 MW, the systems are adjusted to obtain a capacity range of \( 14 < \text{capacity} < 15 \text{ MW} \).

## Design system 1
The inverter is manufactured in China and as an AC output of 116kW.

![image](https://github.com/user-attachments/assets/b87417e1-cf5e-40d9-9d30-64da88964dd5)

Fig 4: 116kW inverter (ENF Ltd., 2022)

### Specifications Table

| **Specifications**               | **Values**     |
|----------------------------------|----------------|
| Max. DC Voltage                  | 1500 V         |
| Nominal DC Voltage               | 1080 V         |
| Min. DC Voltage to Start Feed In | 650 V          |
| Max. DC Current                  | 150 A          |
| MPP(T) Voltage Range             | 600-1500 V     |
| No. of MPP Trackers              | 6              |
| Efficiency                       | 98.8%          |
| Max. AC Power                    | 116 kW         |
| Nominal AC Power                 | 116 kW         |
| Nominal AC Voltage               | 800 V          |
| Max. AC Current                  | 86.6 A         |
| Cost                             | Rs             |

**Table 4: Specifications Table**


The panel is manufactured in China and the 340 Wp is selected.

![image](https://github.com/user-attachments/assets/f9a0fcbc-4825-45c4-aab9-64b929fa6531)

Fig 5: 340 W PV panel (ENF Ltd., 2022)

### Specifications Table

| **Specifications**              | **Values**        |
|---------------------------------|-------------------|
| Maximum Power (Pmax)            | 340 Wp            |
| Voltage at Maximum Power (Vmpp)  | 37.84 V           |
| Current at Maximum Power (Impp)  | 8.95 A            |
| Open Circuit Voltage (Voc)       | 44.95 V           |
| Short Circuit Current (Isc)      | 9.75 A            |
| Panel Efficiency                 | 17.53 %           |
| **Panel Dimension (H/W/D)**      | **1956x992x40 mm**|
| **Cell Number**                  | **72**            |
| **Temperature Coefficient of Pmax** | **-0.47%/°C**  |
| **Temperature Coefficient of Voc**  | **-0.346%/°C** |
| **Temperature Coefficient of Isc**  | **+0.036%/°C** |

**Table 5: Specifications table**

Calculations for number of panels and inverters were performed on Excel as the values can be altered to match requirements.

### Table 6: Excel Calculations

#### Inverter Specifications

| **Specifications**             | **Values**     | **Units** |
|---------------------------------|----------------|-----------|
| No. of inverters                | 126            |           |
| Min Input Voltage               | 650            | V         |
| Max Input Voltage               | 1500           | V         |
| Max Input Current               | 150            | A         |
| Nominal Output Power            | 116000         | W         |
| Peak Input Power                | 2200000        | W         |
| String Connections              | 6              |           |

#### Module Specifications

| **Specifications**             | **Values**     | **Units** |
|---------------------------------|----------------|-----------|
| Nominal Module Power            | 340            | W         |
| Module Short Circuit Current    | 9.75           | A         |
| MPP Current                     | 8.95           | A         |
| MPP Voltage                     | 37.84          | V         |
| Open Circuit Voltage            | 44.95          | V         |
| MIN # of Panels per String      | 13             |           |
| MAX # of Panels per String      | 31             |           |
| MAX # of Strings per MPPT       | 11             |           |
| Number of Modules per String    | 30             |           |
| Number of Parallel Strings Used | 1,386          |           |
| Number of Parallel Strings per MPPT Used | 3     |           |

#### Power and Temperature Calculations

| **Specifications**             | **Values**     | **Units** |
|---------------------------------|----------------|-----------|
| String Power Rating             | 10200          | W         |
| System Power Rating             | 14137200       | W         |
| Minimum Recorded Temperature    | 17             | °C        |
| Maximum Recorded Temperature    | 30             | °C        |
| Maximum Average Irradiance      | 1250           | W/m²      |
| STC Temperature                 | 25             | °C        |
| STC Irradiance                  | 1000           | W/m²      |
| Tadder                          | 25             | °C        |

#### Temperature Coefficients

| **Temperature Coefficient**     | **Values**     | **Units** |
|---------------------------------|----------------|-----------|
| Voc Temp Coefficient            | -0.33          | %/°C      |
| Vm Temp Coefficient             | -0.36          | %/°C      |
| Isc Temp Coefficient            | 0.1            | %/°C      |
| Pm Temp Coefficient             | -0.23          | %/°C      |

#### String Voltages and Currents

| **Specifications**             | **Values**     | **Units** |
|---------------------------------|----------------|-----------|
| String Voc                      | 1348.5         | V         |
| String Vm                       | 1135.2         | V         |
| System Voc at Low Temp          | 1385           | V         |
| System Vm at High Temp          | 1013           | V         |
| Max Isc under Max S and High Temp | 38           | A         |

#### Power Calculations

| **Specifications**             | **Values**     | **Units** |
|---------------------------------|----------------|-----------|
| Peak Input Power at Max S and Min Temp (Overall) | 179965656 | W         |
| Peak Power at S Max for Each Inverter | 114264.4825  | W         |

#### Requirements

| **Condition**                  | **Status**     |
|---------------------------------|----------------|
| Vocmax < Vdc_max_inverter       | Good           |
| Vmmin > Vdc_min_inverter        | Good           |
| Iscmax < Idcmax                 | Good           |
| Pdcmax < Pdc_max_inverter       | Good           |

**Table 6: Excel Calculations**
