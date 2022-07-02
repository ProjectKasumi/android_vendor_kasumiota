Okay so this one is rather a weird one.

What I've focused on for this one is trying to relocate overlayed init
scripts inside /product partition.

But alongside, as @aScordino recommended, I have also set a config in
Lineage SDK telling all apps using it that we have "notch" so that they
won't try to draw to the center of status bar. Including clock and
network status indicator.

I have also migrated Kasumi trees into Kasumi-Devices GitHub organization
since the next build will most probably be official.

Let's hope this one boots at least. Enjoy!
                       Beru "Stella" Hinode

-----------------------------------------------------------------------

```
3f726c3 (HEAD, m/kasumi-v1, devices/kasumi-v1) rosemary/overlay-lineage: Set `config_haveNotch` overlay to true
4b7fe06 rosemary/rootdir: Build modified init scripts into vendor_overlay
```
