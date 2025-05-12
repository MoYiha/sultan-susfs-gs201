Builds of Sultan Kernel with KernelSU Next and SUSFS. Only for Google Pixel 7/Pro (gs201).

# Changes to original repo
* Doesn't state custom kernel name by default (no Sultan/Wild in localversion; just kernel version to keep things clean).
* Backported stability fixes from latest Sultan upstream:
  - [bcmdhd: Downgrade the DPC thread from SCHED_FIFO to SCHED_NORMAL](https://github.com/kerneltoast/android_kernel_google_zuma/commit/501ce3dcda81231fa932eb663f1537131bf3d6a5) (fixed visual stutters while connected to certain WiFi networks)
  - [cpufreq/sched: Fix the usage of CPUFREQ_NEED_UPDATE_LIMITS](https://github.com/kerneltoast/android_kernel_google_zuma/commit/87059250443a97b07e2133561815b7623782d819) (fixed some types of CPU thermal throttling not working)

# Credits
* [KernelSU Next developers and contributors.](https://github.com/KernelSU-Next/KernelSU-Next)
* [kerneltoast](https://github.com/kerneltoast) for his amazing job on Sultan Kernel.
* [simonpunk](https://gitlab.com/simonpunk/susfs4ksu.git) for susfs4ksu.
* [sidex15](https://github.com/sidex15) for module significally simplifying work with susfs.
* [TheWildJames](https://github.com/TheWildJames) for all base of this repo and scripts with patches.
