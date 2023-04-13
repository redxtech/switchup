# switchup
> switchup is a command line tool for downloading and preparing SD cards for modded switches.

## usage
`switchup` comes with many options for configuring which tools will end up on your modded switch.
most are enabled by default, and passing their flag will disabled them. the ones that are disabled by
default will be enabled if their flag is passed.

```
Usage: switchup -[options]
  -c: skip cleanup
  -d: omit DBI
  -e: include emuNAND
  -f: omit fastCFWswitch
  -g: omit Goldleaf
  -h: include HDR
  -k: keep folder (if zipping)
  -l: omit Lockpick_RCM
  -t: omit Training Mod
  -w: omit WiFi Latency Mod
  -z: zip output a zip

# Example (omit Goldleaf, include HDR, output a zip):
switchup -ghz
```

## included content

|Name|Location|Flag|Enabled by default|
---------------------------------------
|Atmosphere|(https://github.com/Atmosphere-NX/Atmosphere)[GitHub]|`N/A`|`yes`|
|Hekate|(https://github.com/CTCaer/hekate)[GitHub]|`N/A`|`yes`|
|Sigpatches|(https://sigmapatches.coomer.party/sigpatches.zip)[Website]|`N/A`|`yes`|
|Skyline|(https://github.com/skyline-dev/skyline)[GitHub]|`N/A`|`yes`|
|ARCropolis|(https://github.com/Raytwo/ARCropolis)[GitHub]|`N/A`|`yes`|
|WiFi Latency Mod|(https://github.com/blu-dev/arena-latency-slider)[GitHub]|`-w`|`yes`|
|Training Modpack|(https://github.com/jugeeya/UltimateTrainingModpack)[GitHub]|`-t`|`yes`|
|fastCFWswitch|(https://github.com/Hartie95/fastCFWswitch)[GitHub]|`-f`|`yes`|
|Tesla Overlay|(https://github.com/WerWolv/Tesla-Menu)[GitHub]|follows `-f`|`yes`|
|nx-ovlloader|(https://github.com/WerWolv/nx-ovlloader)[GitHub]|follows `-f`|`yes`|
|HewDraw Remix|(https://github.com/HDR-Development/HDR-Releases)[GitHub]|`-h`|`no`|
|Smashline Hook|(https://github.com/blu-dev/smashline_hook)[GitHub]|follows `-h`|`no`|
|DBI|(https://github.com/rashevskyv/dbi)[GitHub]|`-d`|`yes`|
|Goldleaf|(https://github.com/XorTroll/Goldleaf)[GitHub]|`-g`|`yes`|
|Lockpick_RCM|(https://github.com/shchmue/Lockpick_RCM)[GitHub]|`-l`|`yes`|
|Blood Falcon Skin (c02 only)|(https://gamebanana.com/mods/308097)[GameBanana]|`N/A`|`yes`|

## todo
- add update flag to only generate atmosphere/hekate/training mod/fastCFWswitch/tesla files
- add tinfoil option
