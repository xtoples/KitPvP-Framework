# KitPvP-Framework
This repository contains a framework built for KitPvP plugins. The main purpose of this project is if I wanted to create a new KitPvP project of some sorts, I can use this framework as a starting base for the plugin I plan to make.

## Feature List
This framework contains the following features

### Easy to use API
The internal API is crucial for the plugin to work. It is how most classes access features such as Profiles.

You can access the API by doing the following:
```JAVA
KitPvPAPI api = KitPvPAPI.getInstance();

// Example
// Get the manager for Profiles
ProfileManager profileManager = api.getProfileManager();
```

### Profiles
Profiles is a custom stats-tracking object where you can store data and will be printed to JSON. This uses the [Gson Library](https://github.com/google/gson).

Each profile contains the following stats:
* Unique ID (The UUID of the Player/Owner of the Profile)
* Kills (an Integer which represents how many kills you have)
* Deaths (an Integer which represents how many deaths you have)
* KillStreak (an Integer which represents how many kills you have had since your last death)
* Best KillStreak (an Integer which represents your best KillStreak of all time)
* Assists (an Integer which represents how many players you have assisted in killing)
* Coins (a Long which represents how much currency you possess)
* Cosmetics Status (an Object which contains 3 enums of your Kill Effect, Kill Message, and Kill Sound)
* Current Kit (an Enum which represents your current kit you have selected)

### Region
Region is a region system which can be used internally without the need of third party region plugins such as WorldGuard. You can use it internally to determine custom conditions for any piece of code you may make.

## Notice
This Mark Down will be expanded upon at a later date. This currently does not cover all the features of the framework.