# Changelog
All notable changes to this project will be documented in this file.

## [Unreleased]
- No unreleased changes so far

## [0.15.0] - 2021-10-06
### Fixed
- Climate settings and start stop

### Changed
- Updated API to 0.21.0

## [0.14.15] - 2021-09-27
### Fixed
- Fixed resetting of parkingposition while driving

### Added
- New attributes: electricRange, gasolineRange

### Changed
- API updated to 0.20.14

## [0.14.14] - 2021-09-23
### Fixed
- Fixed problems coming from changes in the API

### Added
- New images with badges
- New attributes: odometerMeasurement, rangeMeasurements, unitInCar, targetTemperature_F

### Changed
- API updated to 0.20.12

## [0.14.13] - 2021-09-16
### Fixed
- Fixes previous release that did not take new exceptions into account

## [0.14.12] - 2021-09-15
### Added
- Will retry a request 3 times to try to make instable server connection more stable

### Fixed
- Problem when token could not be refreshed

### Changed
- API updated to 0.20.10

## [0.14.11] - 2021-09-10
### Fixed
- Fix if range is corrupted

## [0.14.10] - 2021-09-02
### Fixed
- Allow forbidden (403) return code for parking position
- Continue fetching data even if retrieval for one car fails

### Changed
- API version to 0.20.6

## [0.14.9] - 2021-09-02
### Fixed
- Fixed UnboundLocalError in condition GDC_MISSING

### Changed
- API version to 0.20.5

## [0.14.8] - 2021-09-01
### Fixed
- Fixed parsing mqttport argument

## [0.14.7] - 2021-09-01
### Fixed
- typing error on python 3.7

### Changed
- API version to 0.20.4

## [0.14.6] - 2021-08-30
### Fixed
- Display of consent url fixed

### Added
- Added new error state delayed

### Changed
- API version to 0.20.3

## [0.14.5] - 2021-08-26
### added
- New error messages for parking position
- New error state: fail_ignition_on

### Changed
- API version to 0.20.2

## [0.14.4] - 2021-08-25
### Added
- New error state: fail_vehicle_is_offline
- New status: climatisationSettingsRequestStatus

### Changed
- API version to 0.19.3

## [0.14.3] - 2021-08-20
### Fixed
- Fixed bad gateway error with parking position when car is driving

### Changed
- API version to 0.19.2

## [0.14.2] - 2021-08-19
### Fixed
- Parking position after weconnect API change

### Changed
- API version to 19.1

## [0.14.1] - 2021-08-15
### Added
- Output of version information after startup

## [0.14.0] - 2021-08-15
### Added
- Possibility to set caching time for picture downloads seperately

### Changed
- Longer caching (24h default) for picture downloads

## [0.13.2] - 2021-08-14
### Fixed
- Bug when downloading pictures fails

### Changed
- Better output of version (adds WeConnect-python version to string)
- Updated API to 0.18.3

## [0.13.1] - 2021-07-30
### Fixed
- Fixes charging and climatization controls

### Changed
- Increase API version to 0.15

## [0.13.0] - 2021-07-28
### Added
- Added invalid WindowHeatingState
- Added invalid ChargeMode
- New statuses lvBatteryStatus (seen for ID vehicles), maintenanceStatus for legacy cars (contains milage and km/days until service) added

## [0.12.2] - 2021-07-26
### Changed
- Improved error message when user consent is missing
- More robust against server side errors when refreshing the tokens
- API updated to version 0.13.2

## [0.12.1] - 2021-07-26
### Fixed
- Import of subpackages

## [0.12.0] - 2021-07-26
### Added
- Dummy for maintenance status (currently no data provided, only error messages)
- Added attribute for chargeMode

### Changed
- More compact string formating
- Changed python API to 0.13.0

## [0.11.4] - 2021-07-25
### Fixed
- Fixed crash due to 404 error when retrieving parking position for cars that don't provide parking positions

## [0.11.3] - 2021-07-18
### Fixed
- Fixed crash due to new elements in the WeConnect API

## [0.11.2] - 2021-07-06
### Changed
- Make docker image smaller
- Release docker image dev versions on edge tag

## [0.11.1] - 2021-07-06
### Fixed
- Build error in Docker file

## [0.11.0] - 2021-07-06
### Added
- Possibility to get data from charging stations with --chargingLocation and --chargingLocationRadius
- Possibility to disable data for capabilities with --no-capabilities
- Possibility to get ASCII ART car and status images (can be disabled with --no-pictures)

## [0.10.1] - 2021-07-03
### Fixed
- Bug with addresses fixed in API 0.11.1

### Changed
- Update API to 0.11.1 to use charging station data

## [0.10.0] - 2021-07-03
### Changed
- Update API to 0.11.0

### Fixed
- More robust against null data in API response

## [0.9.0] - 2021-06-28
### Changed
- Update API to 0.10.0 to use access token instead of id token

## [0.8.2] - 2021-06-21
### Fixed
- Potential problem with finding leaf elements by updating API to 0.8.2
- Missing fail status for target operations by updating API to 0.9.

## [0.8.1] - 2021-06-21
### Fixed
- Wrong error message containing unused attribute

## [0.8.0] - 2021-06-21
### Added
- Support for chargeMode attribute by increasing API version to 0.8.0

## [0.7.0] - 2021-06-21
### Added
- Support for singleTimer attribute (party fixes #7)

## [0.6.2] - 2021-06-18
### Fixed
- Fix for issue #6 when the broker publishes old messages after subscribe

### Changed
- Updating API to Version 0.6.2 fixing several small issues

## [0.6.1] - 2021-06-13
### Changed
- Updating API to Version 0.6.1 to fix bug with obervers

## [0.6.0] - 2021-06-11
### Added
- Support for coUsers attribute

### Changed
- Update API version to 0.6.0

## [0.5.2] - 2021-06-10
### Changed
- Update API version to 0.5.2 to fix bug with charging settings

## [0.5.1] - 2021-06-09
### Changed
- Update API version to 0.5.1

## [0.5.0] - 2021-06-09
### Added
- Possibility to change settings and control the vehicle through MQTT messages

### Changed
- API updated to 0.5.0

## [0.4.0] - 2021-06-06
### Added
Send empty message when topic is disabled
### Changed
- Bump API to 0.4.1

### Fixed
- Crash when server responds with unexpected status code

## [0.3.1] - 2021-06-02
### Changed
- Use API version 0.3.2

## [0.3.0] - 2021-05-31
### Added
- More options for MQTT connection (keepalive, tls, ...)

## [0.2.6] - 2021-05-31
### Fixed
- Correctly use timezone
- Fix problem with caching

## [0.2.0] - 2021-05-28
### Fixed
- Improved error messages for missing netrc files

### Added
- Now comes also with a Docker image
- Default value for .netrc file path shown in help
- Improved error messages for missing netrc files
- Improved error handling for login

## [0.1.0] - 2021-05-27
Initial release

[unreleased]: https://github.com/tillsteinbach/WeConnect-mqtt/compare/v0.15.0...HEAD
[0.15.0]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.15.0
[0.14.15]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.14.15
[0.14.14]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.14.14
[0.14.13]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.14.13
[0.14.12]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.14.12
[0.14.11]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.14.11
[0.14.10]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.14.10
[0.14.9]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.14.9
[0.14.8]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.14.8
[0.14.7]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.14.7
[0.14.6]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.14.6
[0.14.5]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.14.5
[0.14.4]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.14.4
[0.14.3]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.14.3
[0.14.2]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.14.2
[0.14.1]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.14.1
[0.14.0]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.14.0
[0.13.2]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.13.2
[0.13.1]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.13.1
[0.13.0]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.13.0
[0.12.2]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.12.2
[0.12.1]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.12.1
[0.12.0]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.12.0
[0.11.4]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.11.4
[0.11.3]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.11.3
[0.11.2]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.11.2
[0.11.1]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.11.1
[0.11.0]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.11.0
[0.10.1]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.10.1
[0.10.0]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.10.0
[0.9.0]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.9.0
[0.8.2]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.8.2
[0.8.1]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.8.1
[0.8.0]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.8.0
[0.7.0]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.7.0
[0.6.2]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.6.2
[0.6.1]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.6.1
[0.6.0]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.6.0
[0.5.2]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.5.2
[0.5.1]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.5.1
[0.5.0]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.5.0
[0.4.0]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.4.0
[0.3.1]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.3.1
[0.3.0]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.3.0
[0.2.6]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.2.6
[0.2.0]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.2.0
[0.1.0]: https://github.com/tillsteinbach/WeConnect-mqtt/releases/tag/v0.1.0
