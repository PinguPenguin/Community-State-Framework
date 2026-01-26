# Community State Framework
Community States Framework (CSF) is a utility mod meant to break up the large files in /map_data/state_regions for ease of modding and deconflicting.

# Intent
Like Community Mod Framework at large, this framework aims to preserve base game behavior by default. If no other mod is used, this framework should be invisible to players. At no point should this framework be used to add or change any content in the game aside from merely splitting the state region files. The goal is to provide modders with more flexibility in modifying state regions and to minimize collisions between mods that touch state regions.

## File Naming
Files are prefixed in a manner that reflects the base game file structure:
- 00_west_europe.txt
- 01_south_europe.txt
- 02_east_europe.txt
- 03_north_africa.txt
- 04_subsaharan_africa.txt
- 05_north_america.txt
- 06_central_america.txt
- 07_south_america.txt
- 08_middle_east.txt
- 09_central_asia.txt
- 10_india.txt
- 11_east_asia.txt
- 12_indonesia.txt
- 13_australasia.txt
- 14_siberia.txt
- 15_russia.txt
- 99_seas.txt

## Updates
CaesarVincens has provided a Powershell script that is able to regenerate the state region files using the base game files as inputs. This is essential for updating CSF should there be any province map/state region changes from PDX.

## Community Engagement
The absolute best place to connect with the project is via the Discord server: [Victoria 3 Mod Co-op](https://discord.gg/XJbqFbHdsM)
