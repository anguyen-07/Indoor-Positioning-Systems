# Indoor-Positioning-Systems

Indoor positioning systems (IPS) use WiFi signals from network access points within a wireless local area network (LAN) to track people and objects inside stores, warehouses, hospitals, and factories. The system requires a reference data set that contains signal strength measurements between wireless mobile devices (i.e. cellular phone, laptop, etc.) and fixed access points (i.e. routers) at known locations within the environment. 

In this analysis, a k-nearest neighbor (kNN) model for the location is trained as a function of the signal strengths between the devices and each access point. This model is used to predict the locations of new, unknown devices based on the detected signals for the device.
