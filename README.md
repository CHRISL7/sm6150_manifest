# Sync

```
repo init -u ssh://git@github.com/chrisl7/sm6150_manifest -b LA.UM.9.1.r1
```

```
repo sync -c -j$(nproc --all) --no-clone-bundle --no-tags --force-sync
```

# Build
```
 . build/envsetup.sh && lunch sm6150-user && ./build.sh -j$(nproc --all) | tee log.xt
```
