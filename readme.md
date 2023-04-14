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
  -n: omit Tinfoil
  -r: include RetroArch
  -t: omit Training Mod
  -w: omit WiFi Latency Mod
  -z: output a zip file

# Example (omit Goldleaf, include HDR, output a zip):
switchup -ghz
```

## included content

|Name|Location|Flag|Enabled by default|
|--- |---     |--- |---               |
|Atmosphere|[GitHub](https://github.com/Atmosphere-NX/Atmosphere)|`N/A`|`yes`|
|Hekate|[GitHub](https://github.com/CTCaer/hekate)|`N/A`|`yes`|
|Sigpatches|[Website](https://sigmapatches.coomer.party)|`N/A`|`yes`|
|Skyline|[GitHub](https://github.com/skyline-dev/skyline)|`N/A`|`yes`|
|ARCropolis|[GitHub](https://github.com/Raytwo/ARCropolis)|`N/A`|`yes`|
|WiFi Latency Mod|[GitHub](https://github.com/blu-dev/arena-latency-slider)|`-w`|`yes`|
|Training Modpack|[GitHub](https://github.com/jugeeya/UltimateTrainingModpack)|`-t`|`yes`|
|fastCFWswitch|[GitHub](https://github.com/Hartie95/fastCFWswitch)|`-f`|`yes`|
|Tesla Overlay|[GitHub](https://github.com/WerWolv/Tesla-Menu)|follows `-f`|`yes`|
|nx-ovlloader|[GitHub](https://github.com/WerWolv/nx-ovlloader)|follows `-f`|`yes`|
|HewDraw Remix|[GitHub](https://github.com/HDR-Development/HDR-Releases)|`-h`|`no`|
|Smashline Hook|[GitHub](https://github.com/blu-dev/smashline_hook)|follows `-h`|`no`|
|DBI|[GitHub](https://github.com/rashevskyv/dbi)|`-d`|`yes`|
|Goldleaf|[GitHub](https://github.com/XorTroll/Goldleaf)|`-g`|`yes`|
|Tinfoil|[Website](http://tinfoil.io)|`-n`|`yes`|
|Lockpick_RCM|[GitHub](https://github.com/shchmue/Lockpick_RCM)|`-l`|`yes`|
|Blood Falcon Skin (c02 only)|[GameBanana](https://gamebanana.com/mods/308097)|`N/A`|`yes`|
|RetroArch|[Website](https://www.retroarch.com)|`-r`|`no`|

## dependencies
there aren't too many programs required to run `switchup`.

- `bash` (or any posix compliant shell) - to run the script.
- `curl` - to download content.
- `gh` - to download content from github releases.
- `unzip` - to extract content from github releases
- `p7zip` - to extract retroarch zip

## todo
- add update flag to only generate atmosphere/hekate/training mod/fastCFWswitch/tesla files
- add [TinWoo](https://github.com/mrdude2478/TinWoo)
- add [aio-switch-updater](https://github.com/HamletDuFromage/aio-switch-updater)
- add [ovl-sysmodules](https://github.com/WerWolv/ovl-sysmodules)
- add [Status-Monitor-Overlay](https://github.com/masagrator/Status-Monitor-Overlay)
- add [sys-clk](https://github.com/retronx-team/sys-clk) and/or [sys-clk-overlay](https://github.com/SunResearchInstitute/sys-clk-Overlay)
- add [nx-btred](https://github.com/plutooo/nx-btred)
- add [MissionControl](https://github.com/ndeadly/MissionControl) and/or [sys-con](https://github.com/cathery/sys-con)?
- add [Amiigo](https://github.com/CompSciOrBust/Amiigo) and/or [emuiibo](https://github.com/XorTroll/emuiibo)
