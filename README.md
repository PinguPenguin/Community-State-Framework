# Community-States-Framework
Community States Framework (CSF) is a mod meant to break up the large files in /map_data/state_regions for ease of modding and deconflicting.

Workshop Page: https://steamcommunity.com/sharedfiles/filedetails/?id=3654153829

## Intent and Scope:
This mod does not add or change any content and is meant solely to aid modders. In the base game, the files in the map_data/state_regions directory cover dozens of state regions each. This is a large compatibility issue since flavor mods that want to edit state regions in the same file will need a compatch.

CSF seeks to mitigate this by breaking up these large files. This means that if your intent is to change resource distribution, you can edit the singular file for that state region instead of locking up dozens of state regions for small edits.

## Usage:
Place this mod as high as possible in your load order! This mod will replace the entire /map_data/state_regions directory, after which any downstream mod files can be loaded back in.

To modify a state region under this framework, replace the specific state region file that you intend to modify. For example, if your intent is to modify `STATE_WALES`, place a file named `00_14_STATE_WALES.txt` in your mod that contains your modifications to the `STATE_WALES` state region. Do this for every state region you intend to modify.

Please note that files are prefixed in a manner that reflects the base game file structure:
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

## Detection:
CSF contains the trigger `csf_is_active_trigger`. This will evaluate to true if CSF is present.