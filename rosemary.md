Another build, another fixup batch.

This one is now official of course!.. with a downside.
I had to kind of *abuse* my role as lead developer and add a flag for
official maintainers so they can ignore signature requirement and build
official without signing. Though don't worry. Even if we define the flag
as true, we're still obliged to keep keys cloned as a sanity check.

THAT ASIDE THOUGH, this build rather focuses on some ricing and doesn't
add anything functional device-side except an attempt to fix lowest
brightness by ~~kanging~~importing display steps from the Pixel 5.

The ricings I have done;

If you can read, you'll see first user experience for fingerprint
enrollment won't tell you to locate the fingerprint sensor on your
device's back, but instead on the right side of your device. If you use
your device from its back instead of front (Literally how), then it's
your problem because regular people use their devices with screen facing
them.

Not that you would notice if you don't have developer options enabled
but I have hidden sRGB option from there since it works only on Google
Nexus/Pixel devices and not on others, even if we set the device props
to it because that's rather hardware thing.

And next up, new stuff: If you have seen the poll I have run before,
maybe you know what's to come but let me tell anyway. This build ships
Lawnchair and AdAway in it! Means you can use more features for home
screen and block ads on the fly! Keep in mind some features might
require root and be unavailable without - Such as DT2S on Lawnchair
and battery efficient VPN-less ad blocking on AdAway.

Vanilla and AuroraOSS builds are soon to come and will be released
as OTA to each build types.

Enjoy!

                       Beru "Stella" Hinode

-----------------------------------------------------------------------

`vendor/kasumi`

```
46f8d190 (HEAD, m/kasumi-v1, kasumi/kasumi-v1) build/tasks/bandori: Add a flag to not enforce signing on official
```

`device/redmi/rosemary`

```
fbd5f7b (HEAD, m/kasumi-v1, devices/kasumi-v1) rosemary/kasumi: Don't enforce signing
1cdf249 rosemary/kasumi: Add properties for Kasumi add-ons
8b362de rosemary: Set correct location for fingerprint sensor
6742c91 rosemary: Hide sRGB toggle in developer options
784819d rosemary/overlay/RF: Kang brightness values from redfin
a74bbc8 rosemary/prebuilt/unpack-vendor: Don't check if unpack process fails
```
