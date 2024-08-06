# Flight Logs

This folder contains 4 different datasets recorded from various test flights performed during the months of June and July in the Valdemorillo airfield, Madrid (Spain). The aircraft employed was SAETA UC3M's "Roadrunner" prototype, a fixed wing 2.1m wingspan light UAV of 2.3kg. It was manually controlled via radio with a ground pilot.

The format used to name the datasets follow the convention "YYYY-MM-DD". These flights were performed in:


1. 2024-06-16 | Single flight that ended in crash.
2. 2024-06-25 | Single flight that ended in crash.
3. 2024-06-29 | Single flight that ended in crash.
4. 2024-07-07 | Three consecutive successful flights. (Not available in the repository due to the >100Mb file limit. Available upon request)

Two different data adquisition applications were employed. Logs 1, 2 and 4 were recorded with [SensorLog v5.3](https://sensorlog.berndthomas.net/) and follow the "comma-separated-value" standard (csv) with a header that contains the following data:

| **Column Name**                         | **Data Type**       |
|-----------------------------------------|---------------------|
| loggingTime                             | txt                 |
| loggingSample                           | N                   |
| locationTimestamp_since1970             | s                   |
| locationLatitude                        | WGS84               |
| locationLongitude                       | WGS84               |
| locationAltitude                        | m                   |
| locationSpeed                           | m/s                 |
| locationSpeedAccuracy                   | m/s                 |
| locationCourse                          | °                   |
| locationCourseAccuracy                  | °                   |
| locationVerticalAccuracy                | m                   |
| locationHorizontalAccuracy              | m                   |
| locationFloor                           | Z                   |
| locationHeadingTimestamp_since1970      | s                   |
| locationHeadingX                        | µT                  |
| locationHeadingY                        | µT                  |
| locationHeadingZ                        | µT                  |
| locationTrueHeading                     | °                   |
| locationMagneticHeading                 | °                   |
| locationHeadingAccuracy                 | °                   |
| accelerometerTimestamp_sinceReboot      | s                   |
| accelerometerAccelerationX              | G                   |
| accelerometerAccelerationY              | G                   |
| accelerometerAccelerationZ              | G                   |
| gyroTimestamp_sinceReboot               | s                   |
| gyroRotationX                           | rad/s               |
| gyroRotationY                           | rad/s               |
| gyroRotationZ                           | rad/s               |
| magnetometerTimestamp_sinceReboot       | s                   |
| magnetometerX                           | µT                  |
| magnetometerY                           | µT                  |
| magnetometerZ                           | µT                  |
| motionTimestamp_sinceReboot             | s                   |
| motionYaw                               | rad                 |
| motionRoll                              | rad                 |
| motionPitch                             | rad                 |
| motionRotationRateX                     | rad/s               |
| motionRotationRateY                     | rad/s               |
| motionRotationRateZ                     | rad/s               |
| motionUserAccelerationX                 | G                   |
| motionUserAccelerationY                 | G                   |
| motionUserAccelerationZ                 | G                   |
| motionAttitudeReferenceFrame            | txt                 |
| motionQuaternionX                       | R                   |
| motionQuaternionY                       | R                   |
| motionQuaternionZ                       | R                   |
| motionQuaternionW                       | R                   |
| motionGravityX                          | G                   |
| motionGravityY                          | G                   |
| motionGravityZ                          | G                   |
| motionMagneticFieldX                    | µT                  |
| motionMagneticFieldY                    | µT                  |
| motionMagneticFieldZ                    | µT                  |
| motionHeading                           | °                   |
| motionMagneticFieldCalibrationAccuracy  | Z                   |
| activityTimestamp_sinceReboot           | s                   |
| activity                                | txt                 |
| activityActivityConfidence              | Z                   |
| activityActivityStartDate               | txt                 |
| pedometerStartDate                      | txt                 |
| pedometerNumberofSteps                  | N                   |
| pedometerAverageActivePace              | s/m                 |
| pedometerCurrentPace                    | s/m                 |
| pedometerCurrentCadence                 | steps/s             |
| pedometerDistance                       | m                   |
| pedometerFloorAscended                  | N                   |
| pedometerFloorDescended                 | N                   |
| pedometerEndDate                        | txt                 |
| altimeterTimestamp_sinceReboot          | s                   |
| altimeterReset                          | bool                |
| altimeterRelativeAltitude               | m                   |
| altimeterPressure                       | kPa                 |
| IP_Timestamp_since1970                  | s                   |
| IP_en0                                  | txt                 |
| IP_pdp_ip0                              | txt                 |
| deviceID                                | txt                 |
| deviceOrientationTimeStamp_since1970    | s                   |
| deviceOrientation                       | Z                   |
| batteryTimeStamp_since1970              | s                   |
| batteryState                            | R                   |
| batteryLevel                            | Z                   |
| label                                   | N                   |




On another hand, flight Nº3 was recorded with a more simple application, [Engineering Physics Toolbox Sensor Suite](https://apps.apple.com/us/app/physics-toolbox-sensor-suite/id1128914250), and the header contains the following data:

| **Column Name** | **Data Type**    |
|-----------------|------------------|
| time            | (unspecified)    |
| gFx             | (unspecified)    |
| gFy             | (unspecified)    |
| gFz             | (unspecified)    |
| ax              | (unspecified)    |
| ay              | (unspecified)    |
| az              | (unspecified)    |
| wx              | (unspecified)    |
| wy              | (unspecified)    |
| wz              | (unspecified)    |
| Bx              | (unspecified)    |
| By              | (unspecified)    |
| Bz              | (unspecified)    |
| Azimuth         | (unspecified)    |
| Pitch           | (unspecified)    |
| Roll            | (unspecified)    |
| Gain            | (unspecified)    |
| Latitude        | (unspecified)    |
| Longitude       | (unspecified)    |
| Speed (m/s)     | m/s              |



All datasets were obtained through the applications running on an iPhone 13 Pro Max, onboard the aicraft and positioned at the center of gravity. 

The sensors used to record the data are: 

* **Accelerometer**

Type: MEMS accelerometer
Sensitivity: Measures acceleration forces in g (gravitational force)
Limits: Typically up to ±16g

* **Gyroscope**

    Type: MEMS gyroscope

    Sensitivity: Measures angular velocity in rad/s

    Limits: Typically up to ±2000°/s

* **Magnetometer**

    Type: MEMS magnetometer (digital compass)

    Sensitivity: Measures magnetic field strength in µT (microteslas)

    Limits: Typically up to ±1200 µT

* **Barometer**

    Type: MEMS barometer

    Sensitivity: Measures atmospheric pressure in hPa (hectopascals)

    Limits: Accuracy within ±1 hPa

* **GPS/GNSS**

    Type: Global Positioning System and Global Navigation Satellite System receiver

    Sensitivity: Measures geographical location and altitude

    Limits: Accuracy within a few meters, depending on conditions

The reason this adquisition system was used lies in the nature of the aircraft, which was purely experimental, with no track record of successful flights. In order to avoid damaging high-end electronics, an phone was employed until enough guarantees were found to replace it with a more sophisticated approach.
