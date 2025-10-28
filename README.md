```bash
repo init -u https://github.com/dopaemon/android_kernel_manifest.git -b sm8450
```
```bash
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```
