# manifests
local_manifests

# Havoc OS 4.x

### How to build ###

```bash
# Create dirs
$ mkdir aosp ; cd aosp

# Init repo
$ repo init -u https://github.com/PixelExperience/manifest -b eleven-plus

# Clone my local repo
$ git clone https://github.com/FlominatorGD/manifests.git -b aosp-11-universal7580 .repo/local_manifests

#!!!Be sure to remove unwanted local manifest files that arent for your device!!!

# Sync
$ repo sync --no-repo-verify -c --force-sync --no-clone-bundle --no-tags --optimized-fetch --prune -j`nproc` -v

# Build
$ . build/envsetup.sh && brunch aosp_"your-device-name"-"user or userdebug or eng"
```
