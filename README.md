# docker-nodelink

Link to Nodelink:  http://forum.universal-devices.com/forum/113-nodelink/

== What is Nodelink? ==
NodeLink is a console application (runs on a networked computer) which allows communication between various devices and an ISY-994i with firmware >=V5.
NodeLink is a Node Server which creates nodes (virtual devices) within the ISY.
NodeLink runs on a networked computer running 24-7 w/ NodeLink installed (.Net 4.0 Client Profile on Windows, mono for Linux/OSX)
 
NodeLink currently supports the following devices:
- Venstar ColorTouch Thermostats
- Brultech GEM
- Ecobee Thermostats
- Generic Data (formerly ISYLink)

# CHANGELOG
Revision History:
v0.3.0 (2016-01-15)
- Ecobee: Added selection of desired thermostat in profile
- Added support for DSC PowerSeries Alarms
- Added friendlier names for the nodes when being added to the ISY
v0.2.7 (2016-01-05)
- Ecobee: Added schedule type to node variables
- Ecobee: Fixed writing HVAC state
- Ecobee: Only writes changes to first thermostat in portal now (used to be all).  0.2.8 will allow this to be selected.
- Modified max node name size to 9 characters (and no underscore)
- Minor error handling tweaks
- Venstar: Updated HVAC state in ISY
v0.2.6 (2015-12-13)
- Ecobee: Fixed bug writing remote sensor values
- Ecobee: Added request new pin button to web config
- Major re-write to ISY REST code to handle multi-threaded device interaction
v0.2.5 (2015-12-08)
- Fixed bug where system would crash on startup grabbing ISY node list
- Added additional error handling to ISYData loop
v0.2.4 (2015-12-06)
- GEM: Preliminary support for packet format 4, fixes for sending data to the cloud
- Ecobee: Support for 32 sensors, code cleanup, humidity setpoint now displaying properly when using frost control
- Venstar: Added fan counter to the runtime node
v0.2.3 (2015-11-26)
- Fixed bug decoding GEM's ASCII format
- Added enable/disable option for ISY Data sun position (default is disabled)
- Prevent single-use devices from being installed multiple times
v0.2.2 (2015-11-25)
- Fixed bug calculating time-of-use
- Added error handling to sun position calcs
- Removed ISY variable list from startup (not needed anymore) 
v0.2.1 (2015-11-21)
- Added Ecobee thermostat support
- Added ISYLink support
- Added external sensor and filter alert to Venstar
- Other minor fixes
v0.2.0 (2015-11-06)
- Initial public release

