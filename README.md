# Indoor-Positioning-Systems

Indoor positioning systems (IPS) use WiFi signals from network access points within a wireless local area network (LAN) to track people and objects inside stores, warehouses, hospitals, and factories. The system requires a reference data set that contains signal strength measurements between wireless mobile devices (i.e. cellular phone, laptop, etc.) and fixed access points (i.e. routers) at known locations within the environment. 

In this analysis, a k-nearest neighbor (kNN) model for the location is trained as a function of the signal strengths between the devices and each access point. This model is used to predict the locations of new, unknown devices based on the detected signals for the device.

For the data used, the floor plan for the building of the test environment contains only 6 fixed access points, but the data shows 7 access points with roughly the expected number of signals. Two of the media access control (MAC) addresses (00:0f:a3:39:e1:c0 & 00:0f:a3:39:dd:cd) appear to be for the same access point. This study investigates whether including both MAC addresses or swapping one out for the other improves prediction performance (i.e. "c0 & cd","c0-only","cd-only")?
