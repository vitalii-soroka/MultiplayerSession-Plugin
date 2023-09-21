# MultiplayerSession-Plugin

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
  
### Introduction
This GitHub project is a C++ plugin for Unreal Engine Online Steam session creation and joining.


### Technologies used:

The Multiplayer Session plugin is built using the following technologies and tools:
- C++ programming language for the application logic
- 
  
### Features
1.

### Installation:
1. [ ] Download Multiplayer Session plugin.
2. [ ] Create a new Unreal Engine project or have already one.
3. [ ] Add "Plugins" folder inside project folder and place Multiplayer Session plugin folder inside.
4. [ ] Add online Steam Subsystem plugin through UE editor.
5. [ ] In Config folder add to DefaultEngine.ini file the following configurations:
~~~
[/Script/Engine.GameEngine]
+NetDriverDefinitions=(DefName="GameNetDriver",DriverClassName="OnlineSubsystemSteam.SteamNetDriver",DriverClassNameFallback="OnlineSubsystemUtils.IpNetDriver")

[OnlineSubsystem]
DefaultPlatformService=Steam

[OnlineSubsystemSteam]
bEnabled=true
SteamDevAppId=480

[/Script/OnlineSubsystemSteam.SteamNetDriver]
NetConnectionClassName="OnlineSubsystemSteam.SteamNetConnection"
~~~
6. [ ] To cap number of possible players change value in DefaultGame.ini 
~~~
[/Script/Engine.GameSession]
MaxPlayers=100
~~~
7. [ ] Add bInitServerOnClient=true to DefaultEngine.ini [OnlineSubsystemSteam].
~~~
[OnlineSubsystemSteam]
bEnabled=true
SteamDevAppId=480
bInitServerOnClient=true
~~~

### Usage


### Plugin Preview
