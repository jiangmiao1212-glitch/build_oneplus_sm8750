[简体中文](README.md) | **`English`** <br>

[![GitHub](https://img.shields.io/badge/-GitHub|@showdo-181717?logo=github\&logoColor=white\&style=flat-square)](https://github.com/showdo/build_oneplus_sm8750)
[![Telegram](https://img.shields.io/badge/Telegram-Channel-blue.svg?logo=telegram)](https://t.me/qdykernel)
[![Coolapk|Home](https://img.shields.io/badge/Coolapk%7CHome-3DDC84?style=flat-square\&logo=android\&logoColor=white)](http://www.coolapk.com/u/1624571)
[![OnePlus Manifest](https://img.shields.io/badge/OnePlus_Manifest-EB0029?logo=oneplus\&logoColor=white\&style=flat-square)](https://github.com/OnePlusOSS/kernel_manifest) <br><b>This Special thanks for build support to：</b>[![GitHub](https://img.shields.io/badge/-GitHub|@HanKuCha-181717?logo=github\&logoColor=white\&style=flat-square)](https://github.com/HanKuCha/oneplus13_a5p_sukisu)<br>

# This repository provides two build methods

## ✨① Workflow Cloud Build Script Usage

#### Please use a VPN to open the following link:

```bash
https://t.me/qdyKernel/405
```

## 🎁② Local Script Usage

> ⚠️ Note: If you want to use your own forked repository for building, and you changed the repository name when forking, please replace `build_oneplus_sm8750` in the instructions below with your new project name, and change `showdo` in the link below to your GitHub username.
> For example, if your username is `abcd` and your repository name is `123456`, the command would be:
> `git clone https://github.com/abcd/123456.git`

---

```bash
git clone https://github.com/showdo/build_oneplus_sm8750.git
```

```bash
cd build_oneplus_sm8750
```

```bash
chmod +x Build_sm8750.sh
```

```bash
./Build_sm8750.sh
```

---

## For Windows, it is recommended to use WSL

Here is a method to migrate WSL to another drive (such as E drive) to avoid occupying C drive space.

### Steps to migrate WSL2 to another directory

1. Open PowerShell as Administrator and check the current WSL version:

```powershell
wsl -l -v
```

2. Stop all running WSL instances:

```powershell
wsl --shutdown
```

3. Export the Linux distribution you want to migrate (for example, Ubuntu-20.04):

```powershell
wsl --export Ubuntu-20.04 E:/ubuntu.tar
```

4. Unregister the original Linux distribution:

```powershell
wsl --unregister Ubuntu-20.04
```

5. Import the exported distribution into the new directory:

```powershell
wsl --import Ubuntu-20.04 E:\ubuntu\ E:\ubuntu.tar --version 2
```

6. Set the default user:

```powershell
ubuntu2004.exe config --default-user <username>
```

> Please replace `<username>` with the username you set when installing WSL.
> For example, if my username is `qiudaoyu`, the command is:

```powershell
ubuntu2004.exe config --default-user qiudaoyu
```

---
