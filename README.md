LineageOS Manifest for Samsung Galaxy S9/S9+ (star)
===

**Sources**
```bash
repo init -u git://github.com/LineageOS/android.git -b lineage-17.1
mkdir .repo/local_manifests/
curl https://raw.githubusercontent.com/Lukas0610/android/lineage-17.1/default.xml > .repo/local_manifests/star.xml
repo sync -j4
```

**Build**
```bash
source build/envsetup.sh

# For Samsung Galaxy S9 (starlte)
lunch lineage_starlte-userdebug

# For Samsung Galaxy S9+ (star2lte)
lunch lineage_star2lte-userdebug

make bacon -j16
```
