
## TWRP device tree for Galaxy J3 PRO (2017)

For OmniROM from https://github.com/joephyu/android_device_samsung_j3y17lte

Add to .repo/local_manifests/j3y17lte.xml:


```
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
        <remote name="omni_twrp" fetch="ssh://git@github.com/ornamion" />
        <project path="device/samsung/j3y17lte" name="android_device_samsung_j3y17lte" remote="omni_twrp" revision="omni" />
</manifest>
```


Then run `repo sync` to check it out.

To build:

`. build/en*`  
`lunch omni_j3y17lte-eng`  
`make -j5 recoveryimage`  
