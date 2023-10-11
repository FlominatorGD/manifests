# manifests
local_manifests

# Clone my local repo
$ git clone https://github.com/FlominatorGD/manifests.git -b havoc-11-a3y17lte .repo/local_manifests

#!!!Be sure to remove unwanted local manifest files that arent for your device!!!

# Sync
$ repo sync --no-repo-verify -c --force-sync --no-clone-bundle --no-tags --optimized-fetch --prune -j`nproc` -v

# Build
# $ . build/envsetup.sh && brunch omni_"your-device-name"-"user or userdebug or eng"
# to build any device or built "a3y17lte" by following:
$ . build/envsetup.sh && lunch omni_a3y17lte-eng && make recoveryimage 
```
