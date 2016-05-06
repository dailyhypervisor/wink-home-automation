# Author Details

Workflow Developed by: Sid Smith - http://www.dailyhypervisor.com  
Product Documentation available at:   

# Workflow Description

This package is a set of workflows for interacting with the wink API with VMware vRealize ORchestrator. 

![workflow image](http://images.vraexperts.com/wink_workflows.png)

# Workflow Installation

1. Import package into vRealize Orchestrator.
2. Create HTTP-Rest Endpoint and Operations.  (See Rest Operations Info) below for settings.
3. Map HTTP-Rest operations in "Wink REST Operation Elements" Configuration Element.
4. Set client_id, client_secret, username, & password in the "Wink REST Operation Elements". (You must request api access from wink to obtain a client_id
and secret)

# Rest Operations Info

| Operation Name       | Operation Template URL            | Method | ContentType      | Config Element Attrib Name      |
| :------------------- | :-------------------------------- | :----- | :--------------- | :------------------------------ |
| Generate Rest Token  | /oauth2/token                     | POST   | application/json | generateRestToken_restOperation |
| Get Wink Device      | /users/me/{deviceType}            | GET    | application/json | getDevice_restOperation         |
| Activate Wink Object | /{deviceType}/{deviceId}/activate | POST   | application/json | activateDevice_restOperation    |
| Create Wink Object   | /users/me/{deviceType}            | POST   | application/json | createDevice_restOperation      |
| Delete Wink Object   | /{deviceType}/{deviceId}          | DELETE | application/json | deleteDevice_restOperation      |
| Update Wink Device   | /{deviceType}/{deviceId}          | PUT    | application/json | updateDevice_restOperation      |

# Supported devices

  * Light Bulbs
  * Switches
  * Outlets
  * Thermostats
  * Door Locks
  * Garage Door
  
# Current Features

* Lock/Unlock Door Locks
* Turn On/Off Light Bulbs
* Turn On/Off Switches
* Turn On/Off Outlets
* Activate Wink Scenes (Shortcuts)
* Open/Close Garage Doors (Except Chamberlain MyQ)
* Get Smoke Dector Info
* Get Sensor Info
* Get Thermostat Info
* Get Robot Info
  
# To D0

* Add ability to modify thermostat
* Add ability to Open/Close Chamberlain Garage Doors
* Add Support for Quirky Power Strip
* Create Robots
* Create Wink Scenes
* Add Users and assign permissions
* Create Installer
* Add Event Subscription Support

  
# Disclaimer


This workflow and it’s components are provided for informational purposes only without warrant and support .  
Included workflow and components are not intended for production use cases and should be used at your one risk.
