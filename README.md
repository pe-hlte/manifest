# Pixel Experience(CAF base) for Samsung Galaxy note 3 LTE #

### Sync ###

```bash

# Initialize local repository
repo init -u https://github.com/pe-hlte/manifest -b pie-caf

# Sync
repo sync -c -f --force-sync --no-tag --no-clone-bundle -j$(nproc --all) --optimized-fetch --prune
```

### Build ###

```bash

# Set up environment
$ . build/envsetup.sh

# Choose a target
$ lunch aosp_$device-userdebug

# Build the code
$ mka bacon -j$(nproc --all)
```
