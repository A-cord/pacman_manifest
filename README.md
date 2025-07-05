# Buildable repositories for Nothing Phone 2(a)
======================================================================

Starting from zero:
---------
```bash
# cd into your ROM's folder
repo init -u {Rom-Sources}
mkdir -p .repo/local_manifests
curl https://raw.githubusercontent.com/a-cord/pacman_manifest/main/pacman.xml > .repo/local_manifests/pacman.xml
repo sync
```

If you've already synced Rom-Sources:
----------
```bash
# cd into your ROM folder
mkdir -p .repo/local_manifests
curl https://raw.githubusercontent.com/a-cord/pacman_manifest/main/pacman.xml > .repo/local_manifests/pacman.xml
repo sync
```

Add KernelSU-Next:
---------
```bash
cd kernel/nothing/mt6886
curl -LSs "https://raw.githubusercontent.com/rifsxd/KernelSU-Next/next/kernel/setup.sh" | bash -
```
