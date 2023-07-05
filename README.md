# G-VRP-IPD-TW
This is a data repository of the generated instances for a *Green Vehicle Routing Problem with Integrated Pickup and Delivery and Time Windows* (G-VRP-IPD-TW) model. The geographic information data is collected in real time through [Amap](https://www.alibabacloud.com/zh/customers/autonavi) based on a county-level city in China.

-- If you use this data in your scientific article, please cite our SEPS 2023 paper:  
*Tiannuo Yang, Zhongzhu Chu, Bailin Wang. Feasibility on the integration of passenger and freight transportation in rural areas: A service mode and an optimization model. DOI: https://doi.org/10.1016/j.seps.2023.101665*


## Background
Multimodal transport synergistically integrates passenger and freight demand, easing the economic pressure on public transport operators by reducing transportation cost. However, the occurrence of on-demand service changes the nature of scheduling approach during the transportation. In our work, we propose a demand-driven passenger-and-freight-integration service mode (DDPFIS mode) according to the characteristics in rural areas and construct a Green Vehicle Routing Problem with Integrated Pickup and Delivery and Time Windows (G-VRP-IPD-TW) model to assist public transport operators in routing decisions. 

This repository records the problem instances generated dedicated to the above problem, classified with 6 experiments in our work. The geographic data is collected in real-time in Longkou, China. We mainly generate 4 sets of instances (sizes of 8, 12, 16 and 20). Other settings could be seen in Section 5.1 in our paper. 

All numerical results are organized in file [```results.xlsx```](https://github.com/tiannuo-yang/G-VRP-IPD-TW/raw/main/results.xlsx). 

## Usage
### Naming Rule
Instances in our repository are named as:   
```
Num_Type_TW_Mode_C2_Demand_Index.json
```   

For example, an instance with Twenty service stations; Station ratio of 5:5:10; Time windows tightness of 0.1; Integration transportation mode; Initial unit passenger service cost; Initial demand amount; Index 1 for current setup; can be represented as:
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
- "c_4": driver’s wage per minute
- "phi_0": fuel consumption rate with no load
- "yita": fuel consumption coefficient per unit load weight
- "omega": average weight of passengers
- "Q": maximum load of the vehicle, including the weight of passengers and freight 
- "Q_h": maximum passenger capacity of the vehicle
- "M": an arbitrary large constant
- "N_s": set of all service stations
- "N": set of all staions (include service center)
- "K": set of all vehi
- "ser_node": service nodes chosen from all data
- "ser_class": corresponding class of service stations
- "d_h_i": number of boarding passengers at i
- "p_h_i": number of alighting passengers at i
- "d_g_i": weight of deliveredfreight at i
- "p_g_i": weight of picked up freight at i
- "D_h": total number of boarding passengers
- "P_h": total number of alighting passengers
- "D_g": total weight of deliveredfreight
- "P_g": total weight of picked up freight
- "s_i": service duration at i
- "a_i": early limit of time window at i
- "b_i": late limit of time window at i
- "delta_ij": distance from i to j
- "t_ij": travel time from i to j

## Contributors
This work is contributed by these scholars:  
*Tiannuo Yang, <tiannuo_yang@126.com>  
Zhongzhu Chu, <chuzhongzhu@126.com>  
Bailin Wang, <wangbl@ustb.edu.cn>  

Feel free to discuss article-related issues with us.
