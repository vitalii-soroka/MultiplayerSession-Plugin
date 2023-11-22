# Multiplayer Session-Plugin

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)

### Introduction
This GitHub project is a C++ plugin for creating, finding, and joining Unreal Engine Online Steam sessions.

### Technologies used:

The Multiplayer Session plugin is built using the following technologies and tools:
- C++ programming language for the application logic
- Unreal Engine 5 Online Steam subsystem for multiplayer connection.
  
### Features
1. Easy to use multiplayer with Steam.
2. The built-in User Widget Menu with main functionality.
3. Host or find online sessions.

### Installation:
1. [ ] Download Multiplayer Session plugin.
2. [ ] Create a new Unreal Engine project or have already one.
3. [ ] Add the "Plugins" folder inside the project folder and place the Multiplayer Session plugin folder inside.
4. [ ] Add online Steam Subsystem plugin through UE editor.
5. [ ] In the Config folder add to DefaultEngine.ini file the following configurations:
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
6. [ ] To cap the number of possible players change the value in DefaultGame.ini 
~~~
[/Script/Engine.GameSession]
MaxPlayers=100
~~~
7. [ ] Add bInitServerOnClient=true to DefaultEngine.ini [OnlineSubsystemSteam]. Note that the plugin uses "SteamDevAppId=480" by default.
~~~
[OnlineSubsystemSteam]
bEnabled=true
SteamDevAppId=480
bInitServerOnClient=true
~~~

### Usage


### Plugin Preview
