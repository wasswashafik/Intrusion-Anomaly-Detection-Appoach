Data Description 
GPS spoofing and jamming are common attacks against the UAV, however, conducting these experiments for research can be difficult in many areas. 
This dataset consists of a logs from a benign flight as well as one where the UAV experiences GPS spoofing and jamming. 
The Keysight EXG N5172B signal generator is used to provide the true coordinates as a location in Shanghai, China.


GPS spoofing: A Great Scott Gadgets HackRF software-defined radio is used with the GPS-SDR-SIM tool 
(https://github.com/osqzss/gps-sdr-sim) to broadcast 30.286502,120.032669. 

GPS jamming: Jamming is done by broadcasting white guassian noise using the HackRF, with an amplitude of 0.3 and a gain of -48dB.

Instructions: 
PX4 Autopilot v1.11.3 (https://px4.io) is used for all experiments, running on Pixhawk 4 flight controller (PX4_FMU_V5) and Pixhawk GPS receiver. 
The UAV frame is the Holybro S500. QGroundControl (v4.0.9) is used for GCS (http://qgroundcontrol.com). 

Full flight data is contained in ULOG files (https://dev.px4.io/v1.9.0/en/log/ulog_file_format.html)
