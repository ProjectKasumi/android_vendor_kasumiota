Now this one is something interesting. I have done some attempts to fix
brightness as well as switch to enforcing for now! From now on, all
builds of Kasumi for Rosemary will be enforcing -- Just try not to break
it. ;)

I have also removed a commit I thought was addressing some SEL denials
but apparently isn't very good of use and sometimes even breaking some
features!

Before you ask, yes this build should bring back ambient display and AOD
too.

Enjoy!
                       Beru "Stella" Hinode

-----------------------------------------------------------------------

`device/redmi/rosemary`


```
b503e03 (HEAD, m/kasumi-v1, devices/kasumi-v1) rosemary/BC: Switch to enforcing
501f44f rosemary/overlay: Kang brightness values from `redfin`
cc7934b Revert "rosemary/sepolicy/private: Sort some denials out"
ff8bb75 rosemary/kasumi.mk: Update product info from stock
```
