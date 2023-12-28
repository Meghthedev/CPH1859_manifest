# Local Manifests #
Just grab the manifest and sync to get device sources

### LineageOS ###

Required patches for IMS: https://gerrit.pixelexperience.org/q/topic:%22mediatek-ims%22+(status:open%20OR%20status:merged)

```bash

# Grab Local Manifest
curl -o .repo/local_manifests/local_manifests.xml https://raw.githubusercontent.com/realme-mt6771-devs/local_manifest/13/13.xml --create-dirs

# Sync
repo sync -j$(nproc --all) --force-sync
```
