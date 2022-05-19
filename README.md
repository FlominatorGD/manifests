# manifests
local_manifests

# Havoc OS 4.x

### How to build ###

```bash
# Create dirs
$ mkdir havoc ; cd havoc

# Init repo
$ repo init -u https://github.com/Havoc-OS/android_manifest.git -b eleven

# Clone my local repo
$ git clone https://github.com/FlominatorGD/manifests.git -b havoc-11-a3y17lte .repo/local_manifests

#!!!Be sure to remove unwanted local manifest files that arent for your device!!!

# Sync
$ repo sync --no-repo-verify -c --force-sync --no-clone-bundle --no-tags --optimized-fetch --prune -j`nproc` -v

# Build
$ . build/envsetup.sh && brunch havoc_"your-device-name"-"user or userdebug or eng" to build any device or built "a3y17lte" by following:
$ . build/envsetup.sh && brunch havoc_a3y17lte-user
```
![Screenshot_20220519-161445_Chrome](https://user-images.githubusercontent.com/75490337/169401335-e8c5cf47-2b3f-4d16-9d23-69fb5a56d208.png)
