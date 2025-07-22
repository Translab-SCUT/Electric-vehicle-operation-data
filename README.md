# Real-World Battery Dataset Description and Modeling

## Data acquisition method:
The vehicle onboard sensor signals, including temperature, current, voltage, and vehicle-level signals, are transmitted to the Battery Management System (BMS) via the Controller Area Network (CAN) bus. Subsequently, 
the data are forwarded by the onboard telematics unit (T-BOX) to the signal base station at a fixed sampling frequency. The base station then transmits the collected data to the Original Equipment Manufacturer (OEM) and the big data monitoring platform for storage. 
The publicly available dataset utilized in this study includes the following variables: data sampling timestamp, vehicle speed, charging status, accumulated mileage, total voltage, current, state of charge (SOC), and cell-level parameters such as minimum and maximum cell voltages and temperatures.

## Explanation of data table headers

The publicly available dataset used in this study contains the following variables:

| Variable Name | Description |
| -------------- | ----------- |
| Time | Timestamp of data acquisition |
| vhc_speed | Vehicle speed (km/h) |
| charging_signal | Charging status indicator: 3 = driving mode, 1 = charging mode |
| vhc_totalMile | Accumulated driving mileage (km) |
| hv_voltage | Total voltage of the battery pack (V) |
| hv_current | Total current of the battery pack (A) |
| bcell_soc | State of Charge (SOC) |
| bcell_maxVoltage | Maximum cell voltage within the battery pack (V) |
| bcell_minVoltage | Minimum cell voltage within the battery pack (V) |
| bcell_maxTemp | Maximum cell temperature (°C) |
| bcell_minTemp | Minimum cell temperature (°C) |


## Vehicle Information

| Vehicle number | Vehicle type     | Battery material | Initial rated capacity (Ah) | Number of data points | Cumulative Mileage (km) | Sampling frequency (Hz) |
|----------------|------------------|-------------------|-----------------------------|-----------------------|-------------------------|-------------------------|
| Vehicle#1      | Passenger vehicle | NCM              | 150                         | 954754                | 69043                   | 0.1                     |
| Vehicle#2      | Passenger vehicle | NCM              | 150                         | 998243                | 73950                   | 0.1                     |
| Vehicle#3      | Passenger vehicle | NCM              | 160                         | 997098                | 79440                   | 0.1                     |
| Vehicle#4      | Passenger vehicle | NCM              | 160                         | 1150999               | 96279                   | 0.1                     |
| Vehicle#5      | Passenger vehicle | NCM              | 160                         | 1096073               | 114413                  | 0.1                     |
| Vehicle#6      | Passenger vehicle | NCM              | 160                         | 501031                | 27318                   | 0.1                     |
| Vehicle#7      | Passenger vehicle | LFP              | 120                         | 5304111               | 32496                   | 0.5                     |
| Vehicle#8      | Electric bus      | LFP              | 645                         | 675236                | 82668                   | 0.1                     |
| Vehicle#9      | Electric bus      | LFP              | 645                         | 443806                | 43988                   | 0.1                     |
| Vehicle#10     | Electric bus      | LFP              | 505                         | 715956                | 27677                   | 0.1                     |

NCM refers to Nickel Cobalt Manganese lithium-ion batteries, while LFP refers to Lithium Iron Phosphate batteries
Cumulative mileage refers to the total distance traveled by the vehicle within the scope of this dataset.

## Battery Pack Structure

Battery pack structure: Owing to confidentiality constraints imposed by the data platform and OEM manufacturers, the structural details of some vehicle battery packs remain undisclosed. Consequently, 
we have released only the portions of information that were accessible under the current data-sharing agreements.
| Vehicle number | Battery pack structure                  |
|----------------|-------------------------------------------|
| Vehicle#1      | 91 battery cells connected in series     |
| Vehicle#2      | 91 battery cells connected in series     |
| Vehicle#3      | 91 battery cells connected in series     |
| Vehicle#4      | 91 battery cells connected in series     |
| Vehicle#5      | 91 battery cells connected in series     |
| Vehicle#6      | 91 battery cells connected in series     |
| Vehicle#7      | ——                                       |
| Vehicle#8      | ——                                       |
| Vehicle#9      | It contains a total of 360 battery cells |
| Vehicle#10     | It contains a total of 324 battery cells |


Currently, one month of operational data per vehicle has been provided. For access to the full dataset, please contact: mshaojing97@mail.scut.edu.cn






