# 🐧 Embedded Linux: The Ultimate Reference Guide

<p align="center">
  <img src="https://img.shields.io/badge/Embedded-Linux-yellow?style=for-the-badge&logo=linux&logoColor=white" />
  <img src="https://img.shields.io/badge/Kernel-Development-green?style=for-the-badge&logo=linux&logoColor=white" />
  <img src="https://img.shields.io/badge/Device-Drivers-blue?style=for-the-badge&logo=linux&logoColor=white" />
  <img src="https://img.shields.io/badge/Yocto-Project-purple?style=for-the-badge&logo=linux&logoColor=white" />
  <img src="https://img.shields.io/badge/Buildroot-red?style=for-the-badge&logo=linux&logoColor=white" />
</p>

<p align="center">
  <strong>A comprehensive, curated collection of resources, roadmaps, books, tutorials, tools, and projects for mastering Embedded Linux — from beginner to architect level.</strong>
</p>

<p align="center">
  <a href="#-roadmap">Roadmap</a> •
  <a href="#-books">Books</a> •
  <a href="#-video-courses--playlists">Playlists</a> •
  <a href="#-free-training-materials">Free Materials</a> •
  <a href="#-simulators--emulators">Simulators</a> •
  <a href="#-hands-on-projects">Projects</a> •
  <a href="#-communities">Communities</a>
</p>

> Reference style inspired by: [m3y54m/embedded-engineering-roadmap](https://github.com/m3y54m/Embedded-Engineering-Roadmap)

---

## 📋 Table of Contents

- [About This Repository](#-about-this-repository)
- [Who Is This For?](#-who-is-this-for)
- [Roadmap](#-roadmap)
  - [Phase 0: Prerequisites](#phase-0-prerequisites)
  - [Phase 1: Linux Fundamentals](#phase-1-linux-fundamentals)
  - [Phase 2: Toolchains & Cross-Compilation](#phase-2-toolchains--cross-compilation)
  - [Phase 3: Bootloaders (U-Boot)](#phase-3-bootloaders-u-boot)
  - [Phase 4: Linux Kernel](#phase-4-linux-kernel)
  - [Phase 5: Root Filesystem](#phase-5-root-filesystem)
  - [Phase 6: Build Systems (Yocto & Buildroot)](#phase-6-build-systems-yocto--buildroot)
  - [Phase 7: Device Drivers](#phase-7-device-drivers)
  - [Phase 8: Application Development](#phase-8-application-development)
  - [Phase 9: Debugging & Profiling](#phase-9-debugging--profiling)
  - [Phase 10: Advanced Topics](#phase-10-advanced-topics)
- [Books](#-books)
- [Video Courses & Playlists](#-video-courses--playlists)
- [Free Training Materials](#-free-training-materials)
- [Online Courses (Paid)](#-online-courses-paid)
- [Simulators & Emulators](#-simulators--emulators)
- [Hardware Platforms](#-hardware-platforms)
- [Build Systems & Tools](#-build-systems--tools)
- [Hands-On Projects](#-hands-on-projects)
- [Blogs & Websites](#-blogs--websites)
- [GitHub Repositories](#-github-repositories)
- [Conferences & Talks](#-conferences--talks)
- [Communities](#-communities)
- [Interview Preparation](#-interview-preparation)
- [Contributing](#-contributing)

---

## 📖 About This Repository

This repository serves as a **one-stop reference** for anyone learning or working with Embedded Linux. Whether you're a student, a bare-metal embedded engineer transitioning to Linux, or an experienced developer looking to deepen your knowledge, you'll find curated and organized resources here.

**Maintained by:** [Eslam Nasr](https://github.com/eslamnasr) — Embedded Linux Software Engineer, MSc Researcher & Senior Instructor.

> ⭐ If you find this useful, please **star** the repo and **share** it with your network!

---

## 🎯 Who Is This For?

| Level | Description |
|-------|-------------|
| 🟢 **Beginner** | CS/EE students, Arduino/MCU developers wanting to move to Linux |
| 🟡 **Intermediate** | Engineers with basic Linux knowledge, looking to build custom systems |
| 🔴 **Advanced** | Developers working on kernel modules, device drivers, or custom distros |
| 🟣 **Architect** | Lead engineers designing full embedded Linux platforms from scratch |

---

## 🗺 Roadmap

The following roadmap guides you from zero to Embedded Linux Architect. Each phase builds on the previous one.

```

```

---

### Phase 0: Prerequisites

Before diving into Embedded Linux, make sure you have solid foundations:

| Topic | What to Learn | Resources |
|-------|--------------|-----------|
| **C Programming** | Pointers, structures, memory allocation, bitwise operations, function pointers, linked lists | *The C Programming Language* (K&R), *C Programming: A Modern Approach* (K.N. King), *Effective C* (Seacord) |
| **Computer Architecture** | CPU architecture, memory hierarchy, registers, buses, interrupts, DMA | *Computer Organization and Design* (Patterson & Hennessy) |
| **Git & Version Control** | Branching, merging, rebasing, submodules, patch workflows | [Pro Git Book (free)](https://git-scm.com/book) |
| **Basic Electronics** | Voltage, current, GPIO, pull-up/pull-down, logic levels, UART/SPI/I2C basics | *The Art of Electronics* (Horowitz & Hill) |
| **Data Structures** | Linked lists, trees, queues — essential for kernel code | *Data Structures in C* (Kalicharan), MIT 6.006 OCW |

#### C Programming — Full Resource List

**Books (Free)**
- [*The C Programming Language* — Kernighan & Ritchie (K&R)](https://www.amazon.com/Programming-Language-2nd-Brian-Kernighan/dp/0131103628) — the definitive reference
- [*Modern C* — Jens Gustedt](https://modernc.gforge.inria.fr/) — free PDF, covers C11/C17
- [*C Programming For Embedded Systems*](https://freecomputerbooks.com/C-Programming-For-Embedded-Systems.html) — free online

**Books (Paid)**
- *C Programming: A Modern Approach* — K.N. King
- *C in a Nutshell* — Peter Prinz & Tony Crawford (O'Reilly)
- *Effective C* — Robert Seacord — modern secure C

**Online Courses (Free)**
- [CS50x — Harvard (edX)](https://cs50.harvard.edu/x/) — best beginner course, free to audit
- [Embedded Systems using C — Coursera](https://www.coursera.org/learn/embedded-systems-using-c) — free to audit
- [C Programming for Embedded Systems — GeeksforGeeks](https://www.geeksforgeeks.org/electronics-engineering/embedded-c/)

**Online Courses (Paid)**
- [Microcontroller Embedded C Programming: Absolute Beginners — Udemy](https://www.udemy.com/course/microcontroller-embedded-c-programming/)
- [Best Embedded C Courses — Udemy collection](https://forecastegy.com/posts/best-embedded-c-courses-udemy/)
- [Embedded C Programming — Coursera specialization](https://www.coursera.org/courses?query=embedded+c)
- [C Programming for Embedded Systems — Doulos](https://www.doulos.com/training/arm-and-embedded-software/embedded-ccplusplus/c-programming-for-embedded-systems/)
- [C Programming for Embedded Systems — Emertxe](https://www.emertxe.com/trainings/embedded/c-programming-embedded-systems/)

**Practice**
- [exercism.org — C track](https://exercism.org/tracks/c)
- [LeetCode](https://leetcode.com) — algorithms in C

#### Data Structures & Algorithms

- *Data Structures in C* — Noel Kalicharan
- *Introduction to Algorithms (CLRS)* — Cormen et al.
- [MIT 6.006 — Introduction to Algorithms (OCW)](https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-fall-2011/) — free

---

### Phase 1: Linux Fundamentals

| Topic | Resources |
|-------|-----------|
| Linux CLI Mastery | [Bootlin Command Line Tutorial (free)](https://bootlin.com/blog/command-line/), [Linux Journey](https://linuxjourney.com/), [OverTheWire: Bandit](https://overthewire.org/wargames/bandit/) |
| Shell Scripting | [Bash Guide for Beginners](https://tldp.org/LDP/Bash-Beginners-Guide/html/), [Advanced Bash Scripting Guide](https://tldp.org/LDP/abs/html/) |
| Linux System Administration | [*The Linux Command Line* — William Shotts (free PDF)](https://linuxcommand.org/tlcl.php), *Linux Pocket Guide* — Daniel Barrett |
| Linux Internals | *How Linux Works* — Brian Ward |
| System Calls & Programming | *The Linux Programming Interface* — Michael Kerrisk |

---

### Phase 2: Toolchains & Cross-Compilation

| Topic | Resources |
|-------|-----------|
| Cross-Compilation Concepts | [Bootlin Embedded Linux slides — Toolchains chapter](https://bootlin.com/doc/training/embedded-linux/) |
| Crosstool-NG | [Official Docs](https://crosstool-ng.github.io/), [Build guide tutorial](https://longervision.github.io/2019/09/06/OperatingSystems/CompilersTools/crosstool-ng/), [BBB guide](https://blog.billvanleeuwen.ca/creating-a-cross-compiling-toolchain-for-beaglebone-black-with-crosstool-ng) |
| ARM Toolchains | [ARM GNU Toolchain Downloads](https://developer.arm.com/downloads/-/arm-gnu-toolchain-downloads) |
| Linaro Toolchain | [Linaro Releases](https://releases.linaro.org/components/toolchain/binaries/) |
| Make | [GNU Make Manual](https://www.gnu.org/software/make/manual/), [*Managing Projects with GNU Make* — free](https://www.oreilly.com/library/view/managing-projects-with/0596006101/) |
| CMake | [CMake Official Tutorial](https://cmake.org/cmake/help/latest/guide/tutorial/), [UPenn Embedded CMake Guide](https://embedded.seas.upenn.edu/Guides/build-systems/cross-compilation-and-toolchain-files/) |

**Additional Cross-Compilation Articles**
- [Mastering Linux Cross-Compilation for Embedded Systems](https://embedded-sbc.com/posts/linux-cross-compilation/)
- [A Master Guide to Linux Cross Compiling — Medium](https://ruvi-d.medium.com/a-master-guide-to-linux-cross-compiling-b894bf909386)
- [Cross-Compilation Toolchains — Medium](https://can-ozkan.medium.com/cross-compilation-toolchains-5e981f7add94)
- [Embedded Linux Toolchains for Cross-Compilation](https://krishworkstech.com/toolchains/)
- [Compiler Tools for Embedded Linux — The New Stack](https://thenewstack.io/compiler-tools-for-embedded-linux-systems/)

---

### Phase 3: Bootloaders (U-Boot)

| Topic | Resources |
|-------|-----------|
| U-Boot Source & Docs | [U-Boot Official](https://u-boot.readthedocs.io/), [U-Boot GitHub](https://github.com/u-boot/u-boot), [Full Docs Tree](https://docs.u-boot.org/) |
| Boot Process Overview | [Bootlin Embedded Linux Training — Bootloader Chapter](https://bootlin.com/training/embedded-linux/) |
| Device Tree Specification | [devicetree.org](https://www.devicetree.org/specifications/) |
| Practical U-Boot Labs | [Bootlin Lab Materials (free)](https://bootlin.com/doc/training/embedded-linux/) |
| 40+ U-Boot Courses | [Class Central](https://www.classcentral.com/subject/u-boot) |

**Platform-Specific U-Boot Guides**
- [U-Boot — AMD/Xilinx Embedded Design Tutorial](https://docs.amd.com/r/en-US/ug1209-embedded-design-tutorial/U-Boot)
- [U-Boot — Texas Instruments Processor SDK (AM335x)](https://software-dl.ti.com/processor-sdk-linux/esd/docs/06_03_00_106/AM335X/linux/Foundational_Components_U-Boot.html)
- [U-Boot — Toradex Developer Center](https://developer.toradex.com/linux-bsp/os-development/boot/u-boot/)
- [U-Boot Overview — ST Wiki STM32MPU](https://wiki.st.com/stm32mpu/wiki/U-Boot_overview)

---

### Phase 4: Linux Kernel

| Topic | Resources |
|-------|-----------|
| Kernel Source | [kernel.org](https://www.kernel.org/), [GitHub mirror](https://github.com/torvalds/linux) |
| Kernel Configuration | `make menuconfig`, `make defconfig` |
| Kernel Internals | *Linux Kernel Development* (Robert Love), *Understanding the Linux Kernel* (Bovet & Cesati), *Linux Kernel Programming* (Kaiwan N. Billimoria) |
| Kernel Newbies | [kernelnewbies.org](https://kernelnewbies.org/) |
| Kernel Documentation | [kernel.org/doc](https://www.kernel.org/doc/html/latest/) |

**Courses (Free)**
- [A Beginner's Guide to Linux Kernel Development (LFD103) — Linux Foundation](https://training.linuxfoundation.org/training/a-beginners-guide-to-linux-kernel-development-lfd103/) — free
- [Bootlin — Kernel & Driver Development (Free Slides + Labs)](https://bootlin.com/training/kernel/)
- [Introduction to Linux Kernel — UT San Antonio Spring 2025](https://spring2025-utsa.kdlp.underground.software/)
- [100+ Kernel Courses — Class Central](https://www.classcentral.com/subject/linux-kernel-development)

**Courses (Paid)**
- [Linux Kernel Internals and Development (LFD420) — Linux Foundation](https://training.linuxfoundation.org/training/linux-kernel-internals-and-development/)
- [Linux Kernel Development Course — Udemy](https://www.udemy.com/course/linux-kernel-development-course/)
- [Introduction to Linux Kernel Development — Udemy](https://www.udemy.com/course/introduction-to-linux-kernel-development/)
- [Linux Kernel Programming & Yocto — Coursera (CU Boulder)](https://www.coursera.org/learn/linux-kernel-programming-yocto-project)

---

### Phase 5: Root Filesystem

| Topic | Resources |
|-------|-----------|
| BusyBox | [busybox.net](https://busybox.net/), [BusyBox FAQ](https://busybox.net/FAQ.html), [Building a Root Filesystem Tutorial](https://embeddedos.github.io/posts/building-a-rootfs/) |
| Init Systems | systemd documentation, BusyBox init, SysVinit |
| Flash Filesystems | [Kernel docs on JFFS2, UBIFS, SquashFS](https://www.kernel.org/doc/html/latest/filesystems/) |
| initramfs | [kernel.org — ramfs/rootfs/initramfs](https://www.kernel.org/doc/html/latest/filesystems/ramfs-rootfs-initramfs.html) |
| Building RootFS from Scratch | [Bootlin Training Labs](https://bootlin.com/doc/training/embedded-linux/), [eLinux Wiki — Root Filesystem](https://elinux.org/Root_File_System) |
| Minimal RootFS (Yocto) | [O'Reilly excerpt](https://www.oreilly.com/library/view/learning-embedded-linux/9781784397395/ch05s03.html) |

---

### Phase 6: Build Systems (Yocto & Buildroot)

| Tool | Official Site | Getting Started |
|------|--------------|-----------------|
| **Yocto Project** | [yoctoproject.org](https://www.yoctoproject.org/) | [Yocto Quick Build](https://docs.yoctoproject.org/brief-yoctoprojectqs/index.html) |
| **Buildroot** | [buildroot.org](https://buildroot.org/) | [Buildroot Manual](https://buildroot.org/downloads/manual/manual.html) |
| **OpenWRT** | [openwrt.org](https://openwrt.org/) | [OpenWRT Build Guide](https://openwrt.org/docs/guide-developer/toolchain/use-buildsystem) |

**Yocto vs Buildroot Quick Comparison:**

| Aspect | Yocto | Buildroot |
|--------|-------|-----------|
| Complexity | High (steep learning curve) | Low (menuconfig-based) |
| Flexibility | Very high (layers, recipes) | Moderate |
| Build Time | Long (hours for first build) | Fast (minutes) |
| Package Mgmt | Supports rpm/deb/ipk | No runtime package management |
| Industry Use | Dominant in production | Great for prototyping |
| Best For | Large, multi-platform products | Small, single-purpose devices |

**Buildroot Tutorials**
- [The First Steps with Buildroot](https://ejaaskel.dev/the-first-steps-with-buildroot/)
- [Buildroot Tutorial — Gateworks](https://trac.gateworks.com/wiki/buildroot)
- [Buildroot Tutorial — Insper](https://insper.github.io/Embarcados-Avancados/Tutorial-HPS-Buildroot/)
- [Bootlin — Buildroot Training (Free Slides + Labs)](https://bootlin.com/training/buildroot/)
- [Yocto vs Buildroot — Incredibuild](https://www.incredibuild.com/blog/yocto-or-buildroot-which-to-use-when-building-your-custom-embedded-systems)

**Yocto Courses (Free)**
- [Bootlin — Yocto & OpenEmbedded Training (Free Slides + Labs)](https://bootlin.com/training/yocto/)
- [200+ Yocto Courses — Class Central](https://www.classcentral.com/subject/yocto-project)
- [Yocto Project — Official Learn Page](https://www.yoctoproject.org/community/learn/)
- [Learning Yocto Part 1 — Medium](https://medium.com/@meronz/learning-yocto-part-1-a989f4340e90)

**Yocto Courses (Paid)**
- [Embedded Linux Platform Development with Yocto (LFD460) — Linux Foundation](https://training.linuxfoundation.org/training/embedded-linux-development-with-yocto-project/)
- [Learn Embedded Linux Using Yocto Project — Udemy](https://www.udemy.com/course/learn-embedded-linux-using-yocto-project/)
- [Linux Kernel Programming & Yocto — Coursera](https://www.coursera.org/learn/linux-kernel-programming-yocto-project)
- [Advanced Embedded Linux Development Specialization — Coursera (CU Boulder)](https://www.coursera.org/specializations/advanced-embedded-linux-development)
- [Yocto Project — E-Labworks](https://e-labworks.com/en/training/ypr/)

---

### Phase 7: Device Drivers

| Topic | Resources |
|-------|-----------|
| Linux Device Drivers (LDD3) | [Free online — LWN.net](https://lwn.net/Kernel/LDD3/), [PDF — Bootlin](https://bootlin.com/doc/books/ldd3.pdf), [O'Reilly Open Book](https://www.oreilly.com/openbook/linuxdrive3/book/), [FreeComputerBooks](https://freecomputerbooks.com/Linux-Device-Drivers-3rd-Edition.html) |
| Modern Driver Development | *Linux Device Driver Development* 2nd Ed — John Madieu (Packt) |
| Kernel Module Programming | [The Linux Kernel Module Programming Guide (free)](https://sysprog21.github.io/lkmpg/) |
| Device Tree for Drivers | [Device Tree Usage — eLinux](https://elinux.org/Device_Tree_Usage), [kernel.org DT docs](https://www.kernel.org/doc/html/latest/devicetree/usage-model.html) |
| Driver Roadmap | [Roadmap to Master Embedded Linux Device Drivers — embitude.in](https://embitude.in/roadmap-to-master-embedded-linux-device-drivers/) |
| Practice Exercises | [LDD3 Training Exercises — GitHub](https://github.com/leos313/ldd3_training) |

**Kernel Subsystem Docs**
- [kernel.org — Driver API](https://www.kernel.org/doc/html/latest/driver-api/)
- [kernel.org — SPI Subsystem](https://www.kernel.org/doc/html/latest/driver-api/spi.html)
- [kernel.org — I2C Subsystem](https://www.kernel.org/doc/html/latest/i2c/)

**Connectivity & Protocol Tutorials**
- [Understanding UART, SPI, I2C, CAN — Blues University](https://dev.blues.io/blog/blues-university-understanding-sensor-interfaces-uart-i2c-spi-can/)
- [Embedded Connectivity: I2C, SPI, UART, CAN Deep Dive](https://www.rapidseasuite.com/blog/embedded-connectivity-a-deep-dive-into-i2c-spi-uart-can)
- [I2C vs SPI vs UART — Total Phase](https://www.totalphase.com/blog/2021/12/i2c-vs-spi-vs-uart-introduction-and-comparison-similarities-differences/)
- [UART vs I2C vs SPI — Seeed Studio](https://www.seeedstudio.com/blog/2019/09/25/uart-vs-i2c-vs-spi-communication-protocols-and-uses/)
- [Understanding UART, SPI, I2C: Practical Guide — MyEmbeddedSystems](https://www.myembeddedsystems.com/blog/understanding-uart-spi-and-i2c-a-practical-communication-protocols-guide/)
- [Intro to UART, SPI, I2C — element14 Community](https://community.element14.com/learn/learning-center/the-tech-connection/w/documents/4664/an-introduction-to-the-uart-spi-and-i2c-communications-protocols)
- [kernel.org — CAN Networking](https://www.kernel.org/doc/html/latest/networking/can.html)

---

### Phase 8: Application Development

| Topic | Resources |
|-------|-----------|
| POSIX Programming | *The Linux Programming Interface* (Michael Kerrisk) |
| System Programming | *Advanced Programming in the UNIX Environment* (Stevens & Rago) |
| Network Programming | *UNIX Network Programming* (W. Richard Stevens) |
| D-Bus | [D-Bus Tutorial](https://dbus.freedesktop.org/doc/dbus-tutorial.html) |

---

### Phase 9: Debugging & Profiling

| Tool | Purpose | Reference |
|------|---------|-----------|
| **GDB / gdbserver** | Remote debugging | [GDB Manual](https://sourceware.org/gdb/current/onlinedocs/gdb/), [GDB — ST Wiki](https://wiki.st.com/stm32mpu/wiki/GDB) |
| **strace** | System call tracing | `man strace` |
| **ltrace** | Library call tracing | `man ltrace` |
| **ftrace** | Kernel function tracer | [Kernel ftrace docs](https://www.kernel.org/doc/html/latest/trace/ftrace.html) |
| **perf** | Performance analysis | [perf wiki](https://perf.wiki.kernel.org/), [kernel.org perf docs](https://www.kernel.org/doc/html/latest/tools/perf/) |
| **eBPF** | Advanced kernel tracing | *Learning eBPF* (Liz Rice) |
| **Valgrind** | Memory leak detection | [valgrind.org](https://valgrind.org/) |
| **KGDB** | Kernel debugger | [Kernel KGDB docs](https://www.kernel.org/doc/html/latest/dev-tools/kgdb.html) |

**GDB & Remote Debugging Tutorials**
- [Debugging an Embedded System: JTAG, SWD, and GDB](https://developers-heaven.net/blog/debugging-an-embedded-system-jtag-swd-and-gdb/)
- [Debugging ARM64 — Day 1 Introduction to Tools](https://pyjamacafe.com/posts/debugging-arm64-day1-different-tools/)
- [Debugging Embedded Projects Remotely — VisualGDB](https://visualgdb.com/tutorials/arm/remote/)
- [Bootlin — Embedded Linux Debugging (Free Slides)](https://bootlin.com/training/)

**OpenOCD & JTAG**
- [OpenOCD Official Site](https://openocd.org)
- [OpenOCD User's Guide PDF](https://openocd.org/doc/pdf/openocd.pdf)
- [OpenOCD — Eclipse Embedded CDT Plugin](https://eclipse-embed-cdt.github.io/debug/openocd/)
- [Configuring OpenOCD for JTAG Debugging — VisualGDB](https://visualgdb.com/tutorials/arm/openocd/)
- [Configuring OpenOCD for Embedded RISC-V Debugging](https://howtech.substack.com/p/configuring-openocd-for-embedded)
- [Debugging with JTAG — Actuated Robots](https://www.actuatedrobots.com/debugging-with-jtag/)
- [OpenOCD + GDB Guide — SJSU Dev Linux](https://sjsu-dev-linux.readthedocs.io/en/latest/rst/guides/debugging-with-openocd-gdb.html)

---

### Phase 10: Advanced Topics

| Topic | Resources |
|-------|-----------|
| Real-Time Linux (PREEMPT_RT) | [RT Linux Wiki](https://wiki.linuxfoundation.org/realtime/start), [ProteanOS PREEMPT_RT Guide (2026)](https://proteanos.com/doc/real-time-linux-preempt-rt-latency-2026/), [Bootlin RT Training Materials](https://bootlin.com/doc/training/preempt-rt/), [RT Linux Explained — LinuxGizmos](https://linuxgizmos.com/real-time-linux-explained/) |
| Xenomai | [Xenomai Official](https://xenomai.org), [Xenomai 3 Overview](https://v3.xenomai.org/overview/), [Xenomai Exercises](https://www.cs.ru.nl/lab/xenomai/exercises_xenomai2.4/ex01/Exercise-1.html) |
| Secure Boot & Security | *Embedded Linux Security* guides, [meta-security (Yocto)](https://git.yoctoproject.org/meta-security) |
| OTA Updates | [Mender.io](https://mender.io/), [RAUC](https://rauc.io/), [SWUpdate](https://sbabic.github.io/swupdate/) |
| Embedded Graphics | [Wayland](https://wayland.freedesktop.org/), DRM/KMS subsystem |
| Containerization | [Balena](https://www.balena.io/), Docker on ARM |
| Linux Networking | [Bootlin Networking Training](https://bootlin.com/training/networking/), *Linux Network Administrator's Guide* |
| RT Courses | [30+ RT Linux Courses — Class Central](https://www.classcentral.com/subject/real-time-linux), [RT Embedded Linux C Programming — The Training Arm](https://thetrainingarm.co.uk/ARM_Embedded_Linux_Programming_Courses/Real_Time_Embedded_Linux_C_Programming.php) |

---

## 📚 Books

### Embedded Linux (Core)

| Book | Author(s) | Level | Focus |
|------|-----------|-------|-------|
| **Mastering Embedded Linux Development** (4th Ed, 2025) | Frank Vasquez, Chris Simmonds | 🟡🔴 | Complete embedded Linux system development (Yocto, Buildroot, kernel, rootfs) |
| **Embedded Linux Primer** (2nd Ed) | Christopher Hallinan | 🟢🟡 | Practical introduction to embedded Linux development |
| **Embedded Linux Systems with the Yocto Project** | Rudolf Streif | 🟡🔴 | Yocto-focused development guide |
| **Exploring BeagleBone** | Derek Molloy | 🟢🟡 | Hands-on with BeagleBone Black |

### Linux Kernel & Drivers

| Book | Author(s) | Level | Focus |
|------|-----------|-------|-------|
| **Linux Kernel Programming** (2nd Ed) | Kaiwan N. Billimoria | 🟡🔴 | Kernel internals, modules, synchronization |
| **Linux Kernel Programming Part 2** | Kaiwan N. Billimoria | 🔴 | Character & block drivers |
| **Linux Device Driver Development** (2nd Ed) | John Madieu | 🟡🔴 | Comprehensive driver development |
| **Linux Device Drivers** (3rd Ed) — **FREE** | Corbet, Rubini, Kroah-Hartman | 🟡🔴 | Classic driver reference [(LDD3)](https://lwn.net/Kernel/LDD3/) |
| **Linux Kernel Development** (3rd Ed) | Robert Love | 🟡 | Kernel design & implementation |
| **Understanding the Linux Kernel** | Bovet & Cesati | 🔴 | Deep kernel internals |
| **Linux Kernel Debugging** | Kaiwan N. Billimoria | 🔴 | Kernel debugging techniques |
| **Linux Kernel Programming** (2025) | Thierry Gayet | 🔴 | Kernel architecture with emphasis on device drivers (USB, PCI, networking) |
| **Linux Driver Development for Embedded Processors** | Alberto Liberal de los Ríos | 🟡🔴 | Embedded-focused driver development |

### Linux System Programming

| Book | Author(s) | Level | Focus |
|------|-----------|-------|-------|
| **The Linux Programming Interface** | Michael Kerrisk | 🟡🔴 | Definitive Linux/UNIX system programming (1500+ pages) |
| **System Programming in Linux** (2025) | Stewart N. Weiss | 🟡🔴 | Hands-on system programming |
| **Advanced Programming in the UNIX Environment** | Stevens & Rago | 🔴 | UNIX system programming classic |
| **Linux System Programming** | Robert Love | 🟡 | System calls, process management, I/O |
| **Linux Network Administrator's Guide** | Tony Bautts et al. | 🟡 | Linux networking (O'Reilly, free online) |

### C Programming (for Embedded)

| Book | Author(s) | Free? | Notes |
|------|-----------|-------|-------|
| *The C Programming Language* (K&R) | Kernighan & Ritchie | No | The definitive C reference |
| *Modern C* | Jens Gustedt | Yes | Covers C11/C17 |
| *C Programming: A Modern Approach* | K.N. King | No | Comprehensive beginner-to-advanced |
| *Effective C* | Robert Seacord | No | Modern secure C programming |
| *C in a Nutshell* | Prinz & Crawford | No | Quick reference (O'Reilly) |

### eBPF & Observability

| Book | Author(s) | Level | Focus |
|------|-----------|-------|-------|
| **Learning eBPF** | Liz Rice | 🟡🔴 | eBPF for observability, networking, security |
| **BPF Performance Tools** | Brendan Gregg | 🔴 | Advanced eBPF performance analysis |
| **Systems Performance** (2nd Ed) | Brendan Gregg | 🔴 | Full-stack Linux performance |

### Real-Time & Algorithms

| Book | Author(s) | Level | Focus |
|------|-----------|-------|-------|
| **Hard Real-Time Computing Systems** | Giorgio Buttazzo | 🔴 | RT theory and scheduling |
| **Introduction to Algorithms (CLRS)** | Cormen et al. | 🟡🔴 | Essential algorithms reference |

### Build Systems & Bootloader

| Book | Author(s) | Level | Focus |
|------|-----------|-------|-------|
| **Embedded Linux Development Using Yocto Project** (3rd Ed) | Otavio Salvador, Daiane Angolini | 🟡 | Yocto Project cookbook |
| **Embedded Linux Development with Buildroot** | Gastón Hillar | 🟡 | Buildroot focused guide |

---

## 🎬 Video Courses & Playlists

### YouTube Playlists (Free)

| Playlist / Channel | Platform | Topics Covered |
|--------------------|----------|----------------|
| [**Embedded Linux Step by Step Using Beaglebone**](https://www.youtube.com/playlist?list=PLErTEd2mIg1xgAhWJCqBO_M85bREEJOGl) — FastBit EBA | YouTube | Complete BBB-based embedded Linux |
| [**Introduction to Embedded Linux** — Digi-Key (Shawn Hymel)](https://www.youtube.com/playlist?list=PLEBQazB0HUyTpoJoZecRK6PpDG31Y7RPB) | YouTube | Buildroot, Yocto, STM32MP1 |
| [**Linux Kernel Programming** — Kaiwan N. Billimoria](https://www.youtube.com/@kaiwanbillimoria) | YouTube | Kernel modules, drivers, debugging |
| [**Derek Molloy — BeagleBone**](https://www.youtube.com/@DerekMolloyDCU) | YouTube | BeagleBone Linux, GPIO, drivers |
| [**Bootlin Conference Talks**](https://www.youtube.com/@Bootlin) | YouTube | Kernel, drivers, build systems, real-time |
| [**The Linux Foundation**](https://www.youtube.com/@LinuxfoundationOrg) | YouTube | Embedded Open Source Summit talks |
| [**Low Level Learning**](https://www.youtube.com/@LowLevelLearning) | YouTube | Kernel, drivers, systems programming |
| [**Low Byte Productions**](https://www.youtube.com/@LowByteProductions) | YouTube | Low-level Linux, OS concepts |
| [**FastBit Embedded Brain Academy**](https://www.youtube.com/@FastbitEmbeddedBrainAcademy) | YouTube | Embedded C, MCU, RTOS, Linux |
| [**Wee-W Stack**](https://www.youtube.com/@WeeWStack) | YouTube | Embedded systems concepts |
| [**LiveOverflow**](https://www.youtube.com/@LiveOverflow) | YouTube | Linux security, exploitation, reverse engineering |
| [**Chris Simmonds — Inner Penguin**](https://www.youtube.com/@innerpenguin) | YouTube | Embedded Linux talks and tutorials |
| [**Embedded Artistry**](https://www.youtube.com/@EmbeddedArtistry) | YouTube | Embedded software best practices |
| **NPTEL** | YouTube | IIT-level systems & OS courses |

### YouTube Channels (Arabic)

| Channel | Topics |
|---------|--------|
| [**Mohamed Youssef**](https://www.youtube.com/@MohamedYoussefEmbedded) | Embedded Linux, Device Drivers (Arabic) |
| [**Ahmed AbdElMawgood**](https://www.youtube.com/@AhmedAbdElMawgood) | Embedded Systems & Linux (Arabic) |

---

## 📄 Free Training Materials

These are **gold-standard** freely available training materials:

| Resource | Provider | Content |
|----------|----------|---------|
| [**Embedded Linux Slides (500+ pages PDF)**](https://bootlin.com/doc/training/embedded-linux/embedded-linux-slides.pdf) | Bootlin | Complete embedded Linux course slides |
| [**Embedded Linux Labs (QEMU)**](https://bootlin.com/doc/training/embedded-linux/embedded-linux-qemu-labs.pdf) | Bootlin | Hands-on labs using QEMU (no hardware needed!) |
| [**Embedded Linux Labs (BeagleBone)**](https://bootlin.com/doc/training/embedded-linux/embedded-linux-bbb-labs.pdf) | Bootlin | Labs on BeagleBone Black |
| [**Embedded Linux Labs (STM32MP1)**](https://bootlin.com/doc/training/embedded-linux/embedded-linux-stm32mp1-labs.pdf) | Bootlin | Labs on STM32MP157 Discovery |
| [**Embedded Linux Labs (BeaglePlay)**](https://bootlin.com/doc/training/embedded-linux/embedded-linux-beagleplay-labs.pdf) | Bootlin | Labs on BeaglePlay |
| [**Linux Kernel Training Slides**](https://bootlin.com/doc/training/linux-kernel/) | Bootlin | Kernel & driver development slides + labs |
| [**Buildroot Training**](https://bootlin.com/doc/training/buildroot/) | Bootlin | Buildroot course materials |
| [**Yocto Training**](https://bootlin.com/doc/training/yocto/) | Bootlin | Yocto Project course materials |
| [**Real-Time Linux Training**](https://bootlin.com/doc/training/preempt-rt/) | Bootlin | PREEMPT_RT training materials |
| [**Networking Training**](https://bootlin.com/training/networking/) | Bootlin | Embedded Linux networking materials |
| [**Bootlin Training Materials (GitHub)**](https://github.com/bootlin/training-materials) | Bootlin | All training source (LaTeX, CC-BY-SA license) |
| [**Embedded Linux Wiki (eLinux)**](https://elinux.org/) | Community | Massive wiki for embedded Linux |
| [**Linux Kernel Newbies**](https://kernelnewbies.org/) | Community | Beginner-friendly kernel resources |
| [**The Linux Documentation Project**](https://tldp.org/) | Community | HOWTOs, guides, FAQs |
| [**ARM Education Embedded Linux Kit**](https://www.arm.com/resources/education/education-kits/embedded-linux) | ARM | Embedded Linux education kit |
| [**Linux From Scratch (LFS)**](https://www.linuxfromscratch.org/) | Community | Build entire Linux system from source |
| [**LFD103 — Beginner's Guide to Kernel Dev**](https://training.linuxfoundation.org/training/a-beginners-guide-to-linux-kernel-development-lfd103/) | Linux Foundation | Free kernel development intro course |
| [**200+ Embedded Linux Courses — Class Central**](https://www.classcentral.com/subject/embedded-linux) | Class Central | Aggregated free & paid courses |
| [**Linux Kernel Mailing List (LKML)**](https://lkml.org/) | Community | Primary kernel development mailing list |

---

## 💰 Online Courses (Paid)

| Course | Platform | Instructor / Provider |
|--------|----------|-----------------------|
| [Embedded Linux Step by Step Using Beaglebone Black](https://www.udemy.com/course/embedded-linux-step-by-step-using-beaglebone/) | Udemy | FastBit EBA (Kiran Nayak) |
| [Linux Device Driver Programming Using Beaglebone Black](https://www.udemy.com/course/linux-device-driver-programming-using-beaglebone-black/) | Udemy | FastBit EBA |
| [Embedded Linux](https://www.udemy.com/course/embedded-linux/) | Udemy | Israel Gbati |
| [Linux Kernel Development Course](https://www.udemy.com/course/linux-kernel-development-course/) | Udemy | — |
| [Introduction to Linux Kernel Development](https://www.udemy.com/course/introduction-to-linux-kernel-development/) | Udemy | — |
| [Learn Embedded Linux Using Yocto Project](https://www.udemy.com/course/learn-embedded-linux-using-yocto-project/) | Udemy | — |
| [Embedded Linux Development (LFD450)](https://training.linuxfoundation.org/training/embedded-linux-development/) | Linux Foundation | Linux Foundation |
| [Linux Kernel Internals and Development (LFD420)](https://training.linuxfoundation.org/training/linux-kernel-internals-and-development/) | Linux Foundation | Linux Foundation |
| [Embedded Linux Platform Dev with Yocto (LFD460)](https://training.linuxfoundation.org/training/embedded-linux-development-with-yocto-project/) | Linux Foundation | Linux Foundation |
| [Introduction to Linux (LFS101x)](https://www.edx.org/learn/linux/the-linux-foundation-introduction-to-linux) | edX | Linux Foundation **(FREE)** |
| [Advanced Embedded Linux Development Specialization](https://www.coursera.org/specializations/advanced-embedded-linux-development) | Coursera | CU Boulder |
| [Linux Kernel Programming & Intro to Yocto](https://www.coursera.org/learn/linux-kernel-programming-yocto-project) | Coursera | CU Boulder |
| [Embedded Systems using C](https://www.coursera.org/learn/embedded-systems-using-c) | Coursera | — |
| [Embedded Linux with QEMU Workshop](https://embeddedonlineconference.com/session/Using_QEMU_to_Get_Started_with_Embedded_Linux) | EOC | Mohammed Billoo |
| [Real-Time Embedded Linux C Programming (RT-PREEMPT & Xenomai)](https://thetrainingarm.co.uk/ARM_Embedded_Linux_Programming_Courses/Real_Time_Embedded_Linux_C_Programming.php) | The Training Arm | — |
| [C Programming for Embedded Systems — Doulos](https://www.doulos.com/training/arm-and-embedded-software/embedded-ccplusplus/c-programming-for-embedded-systems/) | Doulos | — |

---

## 🖥 Simulators & Emulators

You **don't need hardware** to get started! These tools let you practice on your PC.

### QEMU (Quick Emulator) — The Essential Tool

| Resource | Description |
|----------|-------------|
| [**QEMU Official**](https://www.qemu.org/) | Open-source machine emulator supporting ARM, MIPS, RISC-V, x86, etc. |
| [**Bootlin QEMU Labs**](https://bootlin.com/doc/training/embedded-linux/embedded-linux-qemu-labs.pdf) | Full embedded Linux labs using QEMU (no hardware!) |
| [**Embedded Linux from Scratch on QEMU**](https://medium.com/@fprotopapa/embedded-linux-from-scratch-quick-easy-on-qemu-87e761834b51) | Step-by-step: toolchain → kernel → rootfs on QEMU |
| [**Building Embedded Linux with QEMU**](https://devarea.com/building-embedded-linux-system-with-qemu/) | Complete system build: kernel + Buildroot + app |
| [**QEMU ARM Emulation Guide**](https://gist.github.com/luk6xff/9f8d2520530a823944355e59343eadc1) | Detailed guide for ARM emulation on Debian/Ubuntu |

**Quick Start with QEMU:**

```bash
# Install QEMU on Ubuntu/Debian
sudo apt install qemu-system-arm qemu-user-static

# List supported ARM machines
qemu-system-arm -M help

# Boot a kernel on Versatile Express board
qemu-system-arm -M vexpress-a9 -m 512M \
    -kernel zImage \
    -dtb vexpress-v2p-ca9.dtb \
    -nographic \
    -append "console=ttyAMA0"
```

### Other Emulators & Virtual Environments

| Tool | Description | Link |
|------|-------------|------|
| **VirtualBox** | Run full Linux distros on any host OS | [virtualbox.org](https://www.virtualbox.org/) |
| **Docker** | Containerized build environments | [docker.com](https://www.docker.com/) |
| **Renode** | Open-source embedded systems simulator | [renode.io](https://renode.io/) |
| **Wokwi** | Online simulator for ESP32/Arduino (IoT gateway) | [wokwi.com](https://wokwi.com/) |
| **WSL2** | Windows Subsystem for Linux (develop on Windows) | [Microsoft Docs](https://learn.microsoft.com/en-us/windows/wsl/) |

---

## 🔧 Hardware Platforms

Recommended boards for hands-on practice:

| Board | Processor | Price Range | Best For |
|-------|-----------|-------------|----------|
| **BeagleBone Black** | TI AM335x (ARM Cortex-A8) | ~$55 | Classic embedded Linux learning, U-Boot, drivers |
| **BeaglePlay** | TI AM6254 (ARM Cortex-A53) | ~$30 | Modern, affordable, great community |
| **Raspberry Pi 4/5** | Broadcom (ARM Cortex-A72/A76) | ~$35-$80 | Versatile, massive community |
| **STM32MP157 Discovery** | STM32MP157 (Cortex-A7 + M4) | ~$70 | Dual-core (Linux + RTOS), industrial |
| **STM32MP2 Discovery** | STM32MP2 (Cortex-A35 + M33) | ~$99 | Latest ST platform |
| **NXP i.MX93 EVK** | NXP i.MX93 (Cortex-A55 + M33) | ~$100+ | NXP ecosystem, Yocto support |
| **NVIDIA Jetson Nano** | Tegra X1 (ARM Cortex-A57) | ~$150 | AI/ML at the edge + Linux |
| **Pine64 / Rock64** | Rockchip (ARM) | ~$25-$45 | Budget-friendly ARM boards |
| **RISC-V Boards** (VisionFive 2, Milk-V) | RISC-V | ~$40-$100 | Emerging architecture |
| **QEMU (virtual)** | ARM / RISC-V / x86 | Free | All stages — no hardware needed |

> 💡 **No hardware?** Use **QEMU** — Bootlin provides complete labs that work entirely in emulation!

---

## ⚙ Build Systems & Tools

### Build Systems

| Tool | Website | Description |
|------|---------|-------------|
| **Yocto Project** | [yoctoproject.org](https://www.yoctoproject.org/) | Industry-standard embedded Linux build framework |
| **Buildroot** | [buildroot.org](https://buildroot.org/) | Simple, efficient embedded Linux build system |
| **OpenWRT** | [openwrt.org](https://openwrt.org/) | Linux for networking devices (routers, etc.) |
| **ELBE** | [elbe-rfs.org](https://elbe-rfs.org/) | Debian-based embedded Linux builder |
| **PTXdist** | [ptxdist.org](https://www.ptxdist.org/) | Pengutronix's embedded Linux build system |

### Essential Tools

| Tool | Purpose |
|------|---------|
| **Crosstool-NG** | Build cross-compilation toolchains |
| **BusyBox** | Lightweight UNIX utilities for embedded |
| **U-Boot** | Universal bootloader |
| **GDB + gdbserver** | Remote debugging |
| **strace / ltrace** | System/library call tracing |
| **ftrace / perf** | Kernel tracing & performance profiling |
| **OpenOCD** | On-chip debugging via JTAG/SWD |
| **Binwalk** | Firmware analysis & extraction |
| **minicom / picocom** | Serial terminal communication |
| **devmem2** | Direct memory access from userspace |
| **i2c-tools** | I2C bus utilities |
| **spidev-tools** | SPI testing utilities |
| **mtd-utils** | Flash memory management |
| **Mender / RAUC / SWUpdate** | OTA update frameworks |
| **cyclictest** | Real-time latency measurement |

---

## 🚀 Hands-On Projects

Practice makes perfect. Try these projects ordered by difficulty:

### 🟢 Beginner

1. **Boot Linux on QEMU** — Cross-compile kernel, create minimal rootfs with BusyBox, boot on QEMU ARM
2. **Custom Buildroot Image** — Build a minimal Linux image for QEMU or Raspberry Pi using Buildroot
3. **Cross-compile a "Hello World"** — Set up a cross-toolchain and compile/run on target
4. **Serial Console Communication** — Connect to a board via UART, explore the boot log
5. **NFS Root Boot** — Boot kernel via TFTP, mount rootfs via NFS

### 🟡 Intermediate

6. **Build a Yocto Image** — Create a custom Yocto distribution for STM32MP1 or BeagleBone
7. **Write a Character Device Driver** — Create a simple `/dev/mydevice` driver with read/write operations
8. **GPIO Sysfs & libgpiod** — Control LEDs and read buttons from Linux userspace
9. **I2C Sensor Driver** — Write a kernel driver for an I2C temperature sensor
10. **Custom Init System** — Replace systemd with a minimal init using BusyBox init or a custom init program

### 🔴 Advanced

11. **Platform Device Driver** — Write a full platform driver with device tree bindings
12. **Custom Yocto Layer & Recipe** — Create your own meta-layer with custom packages and configurations
13. **OTA Update System** — Implement Mender or SWUpdate-based OTA on a real board
14. **Real-Time Application** — Configure PREEMPT_RT kernel patch and test real-time latency with cyclictest
15. **Boot Optimization** — Reduce boot time from 30s to under 3s on an embedded board
16. **Secure Boot Chain** — Implement signed U-Boot → signed kernel → verified rootfs
17. **Custom SoC Board Bring-Up** — Port U-Boot and Linux to a new custom board (device tree, drivers, BSP)

---

## 🌐 Blogs & Websites

| Website | Focus |
|---------|-------|
| [**Bootlin Blog**](https://bootlin.com/blog/) | Kernel, embedded Linux, conferences, training |
| [**EmbeddexAI**](https://embeddexai.com) | Embedded Systems, Embedded Linux, IoT, AI/ML |
| [**eLinux.org**](https://elinux.org/) | Community wiki for embedded Linux |
| [**LWN.net**](https://lwn.net/) | Linux kernel & community news (premium + free) |
| [**Kernel Newbies**](https://kernelnewbies.org/) | Beginner-friendly kernel info |
| [**Developers Area**](https://devarea.com/) | Embedded Linux tutorials (QEMU, Buildroot) |
| [**Embitude**](https://embitude.in/) | Embedded Linux training & roadmaps |
| [**2net.co.uk (Chris Simmonds)**](https://2net.co.uk/) | Inner Penguin — Embedded Linux blog |
| [**Embedded Related**](https://www.embeddedrelated.com/) | Embedded systems articles & forums |
| [**Yocto Project Blog**](https://www.yoctoproject.org/blog/) | Official Yocto news and tutorials |
| [**Linux Kernel Mailing List Archives**](https://lkml.org/) | Kernel development discussions |
| [**ProteanOS Blog**](https://proteanos.com) | Real-time Linux and embedded systems |

---

## 📂 GitHub Repositories

Essential repos to star and study:

| Repository | Description |
|------------|-------------|
| [**bootlin/training-materials**](https://github.com/bootlin/training-materials) | All Bootlin training slides & labs (CC-BY-SA) |
| [**torvalds/linux**](https://github.com/torvalds/linux) | The Linux kernel source code |
| [**u-boot/u-boot**](https://github.com/u-boot/u-boot) | Universal Boot Loader |
| [**buildroot/buildroot**](https://github.com/buildroot/buildroot) | Buildroot build system |
| [**m3y54m/Embedded-Engineering-Roadmap**](https://github.com/m3y54m/Embedded-Engineering-Roadmap) | Comprehensive embedded systems roadmap |
| [**niekiran/EmbeddedLinuxBBB**](https://github.com/niekiran/EmbeddedLinuxBBB) | FastBit's Embedded Linux on BBB course code |
| [**cirosantilli/linux-kernel-module-cheat**](https://github.com/cirosantilli/linux-kernel-module-cheat) | QEMU + Buildroot + kernel module examples |
| [**derekmolloy/exploringBB**](https://github.com/derekmolloy/exploringBB) | Code from "Exploring BeagleBone" book |
| [**PacktPublishing/Mastering-Embedded-Linux-Programming-Third-Edition**](https://github.com/PacktPublishing/Mastering-Embedded-Linux-Programming-Third-Edition) | Book code & examples |
| [**sysprog21/lkmpg**](https://github.com/sysprog21/lkmpg) | Linux Kernel Module Programming Guide |
| [**linux-kernel-labs**](https://linux-kernel-labs.github.io/) | Interactive kernel labs |
| [**leos313/ldd3_training**](https://github.com/leos313/ldd3_training) | LDD3 driver exercises |
| [**jadonk/beaglebone-getting-started**](https://github.com/jadonk/beaglebone-getting-started) | BeagleBone getting started resources |

---

## 🎤 Conferences & Talks

| Conference | Description | Recordings |
|------------|-------------|------------|
| **Embedded Linux Conference (ELC)** | Premier embedded Linux event | [YouTube - Linux Foundation](https://www.youtube.com/@LinuxfoundationOrg) |
| **Embedded Open Source Summit (EOSS)** | Umbrella event for embedded open-source projects | [Linux Foundation Events](https://events.linuxfoundation.org/) |
| **Embedded World** | Largest embedded systems trade fair (Nuremberg) | Various on YouTube |
| **Yocto Project Summit** | Yocto-focused technical summit | [Yocto Project YouTube](https://www.youtube.com/@YoctoProject) |
| **FOSDEM - Embedded Room** | Free, open-source developer meeting (Brussels) | [fosdem.org](https://fosdem.org/) |
| **Linux Plumbers Conference** | Deep kernel & plumbing topics | [YouTube](https://www.youtube.com/@LinuxPlumbersConference) |
| **Embedded Online Conference** | Virtual embedded systems conference | [embeddedonlineconference.com](https://embeddedonlineconference.com/) |

---

## 💬 Communities

| Community | Platform | Link |
|-----------|----------|------|
| **r/embedded** | Reddit | [reddit.com/r/embedded](https://www.reddit.com/r/embedded/) |
| **r/linux** | Reddit | [reddit.com/r/linux](https://www.reddit.com/r/linux/) |
| **Embedded Linux Wiki** | Forum | [elinux.org](https://elinux.org/) |
| **Linux Kernel Mailing List** | Email | [lkml.org](https://lkml.org/) |
| **Yocto Project Mailing List** | Email | [lists.yoctoproject.org](https://lists.yoctoproject.org/) |
| **Buildroot Mailing List** | Email | [buildroot.org/lists.html](https://buildroot.org/lists.html) |
| **Stack Overflow** | Q&A | Tags: `embedded-linux`, `yocto`, `buildroot`, `device-driver` |
| **Embedded Systems Discord** | Discord | Various servers (search "Embedded Systems") |
| **BeagleBoard.org Forum** | Forum | [forum.beagleboard.org](https://forum.beagleboard.org/) |
| **Raspberry Pi Forums** | Forum | [forums.raspberrypi.com](https://forums.raspberrypi.com/) |
| **LinkedIn Groups** | LinkedIn | "Embedded Linux", "Yocto Project", "Embedded Systems" |

---

## 📝 Interview Preparation

Common topics for Embedded Linux Engineer interviews:

| Category | Key Topics |
|----------|------------|
| **Linux Kernel** | Process vs thread, virtual memory, scheduling, interrupts, system calls, kernel vs userspace |
| **Boot Process** | ROM code → SPL → U-Boot → Kernel → Init → Userspace |
| **Device Drivers** | Character/Block/Network drivers, ioctl, file_operations, device model, platform drivers |
| **Device Tree** | DTS syntax, bindings, overlays, compatible property, phandles |
| **Build Systems** | Yocto layers/recipes/bbappend, Buildroot menuconfig, cross-compilation |
| **Debugging** | GDB remote, strace, ftrace, kernel oops analysis, memory debugging |
| **Filesystems** | ext4, JFFS2, UBIFS, SquashFS, tmpfs, procfs, sysfs, devtmpfs |
| **IPC Mechanisms** | Pipes, FIFOs, shared memory, message queues, semaphores, signals, sockets, D-Bus |
| **Networking** | Socket programming, TCP/UDP, Ethernet, CAN, network namespaces |
| **Memory** | Virtual memory, mmap, kmalloc vs vmalloc, DMA, cache coherency |
| **Real-Time** | PREEMPT_RT, priority inversion, RT scheduling policies, latency analysis |
| **Security** | Secure boot, dm-verity, SELinux, cryptographic frameworks |

---

## 🤝 Contributing

Contributions are welcome! If you know of a great resource that's missing:

1. **Fork** this repository
2. **Create** a branch: `git checkout -b add-resource`
3. **Add** your resource to the appropriate section
4. **Commit**: `git commit -m "Add [resource name]"`
5. **Push**: `git push origin add-resource`
6. **Open** a Pull Request

### Contribution Guidelines

- Ensure links are working and resources are freely accessible (or clearly marked as paid)
- Add a brief description for each resource
- Place resources in the correct section and maintain alphabetical order where applicable
- For books, include author(s), edition, and target level

---

## 📄 License

This repository is licensed under the [MIT License](LICENSE). Feel free to use, share, and contribute!

---

<p align="center">
  <strong>⭐ Star this repo if you found it helpful! ⭐</strong>
  <br><br>
  Made with ❤️ for the Embedded Linux Community
  <br>
  <a href="https://embeddexai.com">EmbeddexAI</a> | <a href="https://github.com/eslamelhefny">GitHub</a> | <a href="https://linkedin.com/in/eslamelhefny">LinkedIn</a>
</p>
