# local_manifests_miatoll

Local manifest for building LineageOS 24.0 for the Redmi Note 9 Pro / 9S / Poco M2 Pro (miatoll).
Link or copy `miatoll.xml` into `.repo/local_manifests/` and run `repo sync`.

```bash
mkdir -p .repo/local_manifests
curl -L https://raw.githubusercontent.com/7829hw/local_manifests_miatoll/lineage-24.0/miatoll.xml -o .repo/local_manifests/miatoll.xml
repo sync -c -j$(nproc --all)
source build/envsetup.sh
breakfast miatoll
m bacon
```
