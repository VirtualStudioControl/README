# README

Start here in case you are overwhelmed by the number of repositories and are unsure how all of those Repositories fit together

## Documentation

## List Of Repositories

List of Repositories and their content in this Organisation:

### VirtualStudio

VirtualStudio is software to connect supported Hardware devices to the actions which should happen once a button is pressed. It is split into the core, handling connected devices and executing the actions attached to the Buttons and other controls, and the Configurator, an UI to assign actions to controls in the core. (In theory you could write the JSON config required by hand, but even for small configurations this can exceed 10.000 lines of JSON, so it is not reccommended). Core and Configurator communicate over an TCP connection, so a supported scenario is running the core on one machine, and then remote configuring the core from another machine using the Configurator

#### Common

[virtualstudio_common](https://github.com/VirtualStudioControl/virtualstudio_common) is a package of common code between Configurator and Code. Currently all plugins can also use code from virtualstudio_common without including it as external library

#### Core

The Core is in the repository [VirtualStudioCore](https://github.com/VirtualStudioControl/VirtualStudioCore). This piece of software creates a common interface for all supported hardware. 

#### Configurator

The Configurator is in the repository [VirtualStudioConfigurator](https://github.com/VirtualStudioControl/VirtualStudioConfigurator). This piece of software enables remote configuration of the Core

#### Plugins

##### DMX Plugin

Plugin for Communication with DMX Relay

##### OBS Websocket Plugin

Plugin for Communication with OBS Studio over the websocket plugin

##### System Functions Plugin

Plugin for basic system functionality like inserting Text at the cursor position or triggering keyboard input at the local machine

### DMX Relay

Relay of TCP packets to supported DMX Interfaces

#### DMXRelay

#### DMXRelayConfigurator

### Libraries

### Other
