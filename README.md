# manifests
local_manifests

# LineageOS 18.1

be aware this is in testing

### How to build ###

```bash
# Create dirs
$ mkdir los18 && cd los18

$ repo init -u https://github.com/LineageOS/android.git -b lineage-18.1

# Clone my local repo
$ git clone https://github.com/FlominatorGD/manifests.git -b lineage-18.1 .repo/local_manifests

# Sync
$ repo sync --no-repo-verify -c --force-sync --no-clone-bundle --no-tags --optimized-fetch --prune -j`nproc` -v

# Build
$ . build/envsetup.sh


$ brunch lineage_a3y17lte-userdebug or eng"
