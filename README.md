# G-VRP-IPD-TW
This is a data repository of the generated instances for a *Green Vehicle Routing Problem with Integrated Pickup and Delivery and Time Windows* (G-VRP-IPD-TW) model. The geographic information data is collected in real time through [Amap](https://www.alibabacloud.com/zh/customers/autonavi) based on a county-level city in China.

If you use this data in your scientific article, please cite our XXXX 2022 paper:  
*Tiannuo Yang, Zhongzhu Chu, Bailin Wang. Is the integration of passenger and freight transportation in rural ares feasible? A new Green Vehicle Routing Problem. DOI:XXX*

## Background

## Usage
### Naming Rule
Instances in our repository are named as:   
```
Num_Type_TW_Mode_C2_Demand_Index.json
```   
For example:
```
20_5510_1_integration_1_1_1.json 
```  




### Attributes
Each instance mainly includes the following attributes:
- "SER_NUM": number of the service stations
- "VEH_NUM": maximum number of the vehicles availbale
- "c_1": unit fuel cost
- "c_2": unit passenger service cost
- "c_3": unit vehicle fixed cost
- "c_4": driver’s wage per mimute
- "phi_0"
- "yita"
- "omega"
- "Q"
- "Q_h"
- "M"
- "N_s"
- "N"
- "K"
- "ser_node"
- "ser_class"
- "d_h_i"
- "p_h_i"
- "d_g_i"
- "p_g_i"
- "D_h"
- "P_h"
- "D_g"
- "P_g"
- "s_i"
- "a_i"
- "b_i"
- "delta_ij"
- "t_ij"

## Contributors