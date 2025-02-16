## Nadeoki's Config
#### a TF2 config for high FPS and optimizations
- optimizing ancient default settings to modern requirements
- removing visual fidelity for FPS gains, commented in gfx.cfg for customizations
- including useful binds and optional mods (including for TFDB Gamemmode)
- including [tfdb Snowball mod](https://github.com/flawfree/tfdbqol?tab=readme-ov-file)
  
#### Install
- download the latest [release](https://github.com/nadeoki/tf2/releases) and 
- place the zip into ``SteamLibrary\steamapps\common\Team Fortress 2\tf\custom``
- unzip. Done. You can delete the zip itself after

#### Launch Options
##### Fullscreen Mode:
> -console -novid -no_texture_stream -nosteamcontroller -nojoy -noff -nohltv +fps_max 500
##### Borderless Windowed Mode:
> -noborder -window -console -novid -no_texture_stream -nosteamcontroller -nojoy -noff -nohltv +fps_max 500

For Borderless to work, you might need to use ``-dxlevel 90``< and disable Fullscreen Optimizations on the tf.exe and tf_win64.exe inside of ``SteamLibrary\steamapps\common\Team Fortress 2``

extended guide on [steamforums](https://steamcommunity.com/sharedfiles/filedetails/?id=3153774281) by blood tribes

#### DX Level 
(add to Launch options (ONCE) remove after opening and closing the game (ONCE)
From JarateKing on the Steam forums:
- ``-dxlevel 80`` = best option for fps, but not stable
- ``-dxlevel 81`` = almost just as good for fps but a lot more stable
- ``-dxlevel 90`` = less fps but higher quality graphics
- ``-dxlevel 95`` = could help fps compared to 91, could hurt, depends on your gpu (the default also)
- ``-dxlevel 98`` = [Only exists for XBOX360](https://docs.comfig.app/9.6.1/tf2/misconceptions/), will fallback to ``-dxlevel 95`` on PC 

Note that dxlevel 80 and 81 remove warpaints / skins, as those are DX9 only. Personally I recommend 90 or 95 depending which works better for you, unless you're running a toaster and really need the extra fps from DX8.

#### Crosshair
If you want to use custom crosshairs, check out [this](https://github.com/hbivnm/Venom-Crosshairs) tool.

#### Networking
Type ``66tick`` or ``128tick`` into the console
to set execute configs specific to server tick rate.
on dodgeball servers that allow 1ms lerp, it is recommended to
type ``tfdb``.
Note that these neccesitate that you actually comment all three of them in 
the autoexec.cfg it uses 128tick by default

#### Dodgeball 128 Tick Networking
for blw adv / saka's db / etc
- ``cl_cmdrate 128``
- ``cl_updaterate 128``
- ``cl_interp 0.0078``
- ``cl_interp_ratio 1``
- ``rate 999999``

![Preview](https://files.catbox.moe/3dnv76.png)
![Preview](https://files.catbox.moe/mi7ikj.png)


### Credits
using resources from [Comanglia](https://www.teamfortress.tv/25328/comanglias-config-fps-guide), [cfg.tf](https://cfg.tf/), a guy called DtGR, [hbivnm's crosshair script](https://github.com/hbivnm), [b4nny](https://steamcommunity.com/id/b4nny), [JarateKing](https://github.com/JarateKing) and [tfdbqol](https://github.com/flawfree/tfdbqol?tab=readme-ov-file)
