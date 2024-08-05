# LineageOS for Samsung Starlte

This project provides a build of LineageOS 21.0 for the Samsung Starlte device.

## Prerequisites
- `repo`
- `git`

## Installation
Follow these steps to set up the project and start building LineageOS for Samsung Starlte.
### 1. Initialize LineageOS repository
```bash
repo init -u https://github.com/LineageOS/android.git -b lineage-21.0 --git-lfs
```
### 2. Clone local manifests
```bash
git clone https://github.com/LOS-starlte/local_manifests.git -b lineage-21 .repo/local_manifests
```
### 3. Sync the repositories
```bash
repo sync
```

## Building LineageOS
Once the repositories are synchronized, follow these additional steps to build LineageOS for the Samsung Starlte.

### 1. Set up the build environment
Run the following command to set up the build environment:
```bash
source build/envsetup.sh
```
### 2. Choose the target device
Specify the Samsung Starlte device for the build:
```bash
breakfast starlte
```
### 3. Start the build
Begin the build process with the following command:
```bash
brunch starlte
