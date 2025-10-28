```bash
docker pull dopaemon/jammy:latest
```
```bash
mkdir -p $HOME/Rebase
```
```bash
chmod -R 777 $HOME/Rebase
```
```bash
docker run -itd -v $HOME/Rebase:/home/dora/Rebase dopaemon/jammy:latest
```
```bash
repo init -u https://github.com/dopaemon/android_kernel_manifest.git -b sm8450
```
```bash
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```
