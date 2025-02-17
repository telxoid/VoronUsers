# Afterburner + LGX

Useful links, info, and models for using the The LGX™ Large Gears eXtruder with Afterburner...

- [Afterburner LGX Mounts](#afterburner-lgx-mounts)
- [Klipper config](#klipper-config)
- [Extra LGX Models](#extra-lgx-models)
  * [LGX Cable Cover](#lgx-cable-cover)
  * [LGX Gear Cover](#lgx-gear-cover)
  * [LGX Lever Cover](#lgx-lever-cover)

---

### Afterburner LGX Mounts

Mounting the LXG to AfterBurner requires some additional mounting plates.  You will need both of `@Nemgrea`'s mounts from Discord:

  * `lgx_AftB_Mount_Front.STL` ([Discord file link](https://cdn.discordapp.com/attachments/635687829254701107/823914498700083220/lgx_AftB_Mount_Front.STL))
  * `lgx_AftB_Mount_Rear.STL` ([Discord file link](https://cdn.discordapp.com/attachments/635687829254701107/823914501405540442/lgx_AftB_Mount_Rear.STL))

These models are pinned in the [#voronuser_mods](https://discord.com/channels/460117602945990666/635687829254701107/823914498808217621) channel on Discord, and can be found in [this message](https://discord.com/channels/460117602945990666/635687829254701107/823914498808217621).

Thanks to `@Nemgrea V2.199 V0.000` and the crew for their efforts designing and testing the mounts, and offering them to the community.

<sub>*Aside: For my own build, I found that my third-party M3x20 screws had a large enough head that the toolhead couldn't mount to the X Carriage assembly properly without a bit more clearance.  If you find yourself in this situation, [this mod of @Nemgrea's mount](STLs/lgx_AftB_Mount_Front-extra_clearance.stl) is nearly identical to the one on Discord but with slightly more clearance for the bottom screws.  Please try the (semi)official one first before using this mod :)*</sub>

### Klipper config

Bondtech has some official documentation for configuring Klipper [here](https://www.bondtech.se/product-category/upgrade-kits/lgx/).  Below is the configuration I am currently running.

```
rotation_distance: 8
microsteps: 16
full_steps_per_rotation: 200

# use either
#    gear_ratio: 44:14, 37:17
#    rotation_distance: 55
# or
#    rotation_distance: 8
# but not both!
```

The `either...or` warning is not from Bondtech, but provided here to honor the memory and sacrifice of my first hotend and save those that may come after from suffering the same fate...

### Extra LGX Models

#### LGX Cable Cover

Besides the mounting parts, most people end up asking about a cable cover.  There are a few posted around Discord, but after seeing [Craxoor's PCB cover](https://github.com/craxoor/VoronMods/tree/master/PCB%20Cover) I designed a similar cover from scratch for use with the LGX.  Note that this cover *does not* work with the toolhead PCB - it just looks similar.

  * [`lgx-cable-cover.stl`](STLs/lgx-cable-cover.stl)

![cable_cover.jpg](images/cable_cover.jpg)

(Cereal not included)

#### LGX Gear Cover

A little cover for the Large Gears on the LGX so it doesn't chew through the fan wires.

  * [`lgx-gear-cover.stl`](STLs/lgx-gear-cover.stl)

![gear_cover.jpg](images/gear_cover.jpg)

#### LGX Lever Cover

Drop-in replacement for the filament pre-tension lever, in case you want a different color:

  * [`lgx-lever-cover.stl`](STLs/lgx-lever-cover.stl)

![lever_cover.jpg](images/lever_cover.jpg)
