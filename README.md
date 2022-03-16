# manifests
local_manifests

# LineageOS-19.0

### How to build ###

```bash
# Create dirs
$ mkdir los19 && cd los19

# Init repo
$ repo init -u https://github.com/LineageOS/android.git -b lineage-19.1

# Clone my local repo
$ git clone https://github.com/FlominatorGD/manifests.git -b lineage-19.0-a3xelte .repo/local_manifests

# Sync
$ repo sync --no-repo-verify -c --force-sync --no-clone-bundle --no-tags --optimized-fetch --prune -j`nproc` -v

# Build
$ . build/envsetup.sh

#!!!Be sure to apply lagacy patches for your device!!!

$ brunch lineage_"your-device-name"-"user or userdebug or eng"
