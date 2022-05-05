 ```mermaid
flowchart TD
terminalStart([Start])
terminalEnd([End])
thresholdSet(distanceThreshold = 50)
setDCMotorPin(DCMotorPin = 1)
currentDistanceReading(distanceRead = response from Sonar)
activatePiezo(write LOW to DCMotorPin)
ifDistanceLessThanThreshold{distanceRead < distanceThreshold>}
terminalStart --> thresholdSet
thresholdSet --> setDCMotorPin
setDCMotor --> currentDistanceReading


 ```
