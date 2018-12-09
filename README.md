# WeatherStation
A project to connect the Buienradar BR-1800 / Fine Offset WH2300 to a home automatisation system by either reading the data transfered on the 868mhz frequency, data read via the data ports on the device or by gathering sensordata.

# Information gathered this far:
- Data is transfered through the 868mhz frequency and uses FSK modulation, Fine Offset has provided an overview of the coded datastream. 
- Internals of the device show multiple connections near its communication chip (poorly readable because of coating RF43S BPS108 1647), indicated are VCC, multiple GND, SDN, SDI, SDO, SCK, NIRQ, NSEL and ANT.
- Analysis of the connections with a logic analyser (LHT00SU1 in combination with Sigrok Pulseview) show data on SD0, SDI, SCK NSEL and NIRQ.
