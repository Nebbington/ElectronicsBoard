 ```mermaid
flowchart TD
terminalStart([Start])
terminalEnd([end])
thresholdSet(distanceThreshold = 50)
setDCMotorPin(DCMotorPin = 1)
currentDistanceReading(distanceRead = response from Sonar)
activatePiezo(write LOW to DCMotorPin)
ifDistanceLessThanThreshold{distanceRead < distanceThreshold>}
 ```
