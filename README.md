# TESLA-Sensor-Selection-
AIM

To select the appropriate sensor for autonomous vehicles based on detection range requirements.

PROCEDURE
Identify available sensors: Camera, Radar, LiDAR
Analyze their detection ranges
Compare sensor capabilities (Camera < Radar < LiDAR)
Check required detection range (80 m)
Select the sensor that satisfies the requirement
Display the selected sensor
CODE
# Required detection range
required_range = 80   # in meters

# Sensor ranges (approximate values)
camera_range = 50
radar_range = 70
lidar_range = 100

# Sensor selection logic
if required_range <= camera_range:
    sensor = "Camera"
elif required_range <= radar_range:
    sensor = "Radar"
else:
    sensor = "LiDAR"

# Output
print("Selected Sensor:", sensor)
OUTPUT

Selected Sensor: LiDAR

RESULT

LiDAR is selected as it satisfies the 80 m detection range requirement and provides higher accuracy compared to Camera and Radar, making it suitable for autonomous driving applications like Tesla Autopilot.
