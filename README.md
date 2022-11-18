# luke_garages

## Due to the lack of time and motivation to fix the currently ongoing issues and implement new features the work on the repository is suspended.

This resource only supports ESX Legacy, other versions of the framework **will not** work without modifying the resource.

Alongside cars, aircrafts and boats are also fully supported with them having their own separate garages and impounds.

The impound has checks in place to prevent vehicle duping.

I used esx_vehicleshop, but the resource should work with anything that follows that databse structure in `owned_vehicles` table.

[Video Showcase](https://www.youtube.com/watch?v=GT2u5uoz7Tc) (From 2.0.0 version)

### Dependencies

- [PolyZone](https://github.com/mkafrin/PolyZone)
- [ox_target](https://github.com/overextended/ox_target) (recommended) or [qtarget](https://github.com/overextended/qtarget) (deprecated)
- [ox_lib](https://github.com/overextended/ox_lib)
- Server game build 1868 or newer\*

Make sure to download the release zip for [ox_lib](https://github.com/overextended/ox_lib/releases/latest) (ox_lib.zip).

### Installation

- Download the resource from releases
- Rename folder to luke_garages
- Drop the luke_garages folder into your resources folder
- Import the .sql file into your database
- Start the resource in your server.cfg

If you wish to add more garages or impounds make sure to follow the provided template and examples in the config.lua file.

Custom vehicles are fully supported, for each custom vehicle you have to add a text entry of it's model and make name (if there isn't one already) into the vehicle_names.lua file which is located in the client folder. I provided an example of this that I used on the GTR in the video.

For any issues or bugs that may occur please open an Issue in the repository. Make sure to describe the issue in detail and how to reproduce it.

PRs are always welcome.

## Setting the game build

\*_Setting the game build is required due to the use of GetMakeNameFromVehicleModel native which was introduced in the game version 1868. If (for whatever reason) you don't want to change from the base build that FiveM comes with, you can remove all the appearances of this native and it's variables from the client file. Otherwise your game will be consistently crashing when trying to open either the garage or the impound._

There are two way sto set your game build:

1. Setting the build in your server.cfg
2. Setting the build in your launch params

Both methods work exactly the same, if you are setting your game build through launch params you will need to add a `+` in front of the command, otherwise you don't need to.

The command you need to use is: `set sv_enforceGameBuild` (example: `set sv_enforceGameBuild 2189`)

Depending on the game build number you choose is the GTA DLC your server is going to be running:

```
1604 - Vanilla
2060 - Casino Heist
2189 - Cayo Perico Heist
2373 - Tuners update
2545 - The Contract update
2699 - Criminal Enterprises update
```
## License

    luke_garages
    Copyright (C) 2022 Luke <https://www.github.com/LukeWasTakenn>

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <https://www.gnu.org/licenses/>.
