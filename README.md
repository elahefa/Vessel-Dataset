## Vessel-Dataset
### By Elahe
This document explores a .csv file which is a vessel dataset of a fleet joined with the vessel operation mode at the time of data generation. It contains the following fields:
*	name: Vessel name
*	longitude_deg: Instantaneous longitude in degrees 
*	latitude_deg: Instantaneous latitude in degrees 
*	speed: Instantaneous speed of the vessel
*	course: Instantaneous course of the vessel
*	in_port: Boolean indicating if the vessel is inside a port area. Does not specify whether the vessel is at berth.
*	OP_CODE_NAME_SHORT: Code for the operation mode as reported by the vessel crew. The operation codes translate as follows: 

| Operation mode | Code	| Description |
| -------------- | ---- | ----------- |
| Canal transit	 |  0	| The vessel is transiting a canal (e.g. Suez or Panama canal). |
| Maneuvering	| 1	| The vessel is maneuvering to/from a port. This is typically slower than sea passage. |
| Idling	| 2	| The vessel is not travelling but is also not at berth. This often occurs if the vessel is waiting, e.g. if there is no available space in the destination port. |
| At Berth	| 3	| The vessel is docked and moored. |
| Sea Passage	| 4	| The vessel is travelling normally to its destination. |

The task is to create a model/set of models for predicting the operation mode.
