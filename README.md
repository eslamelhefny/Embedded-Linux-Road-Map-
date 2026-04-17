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
┌──────────────────────────────────────────────────────────────────────┐
│                    EMBEDDED LINUX ROADMAP                            │
├──────────────────────────────────────────────────────────────────────┤
│                                                                      │
│  Phase 0: Prerequisites                                              │
│  ├── C Programming (advanced: pointers, memory, bitwise ops)        │
│  ├── Basic Electronics & Computer Architecture                       │
│  └── Version Control (Git)                                           │
│                                                                      │
│  Phase 1: Linux Fundamentals                                         │
│  ├── Linux CLI & Shell Scripting (Bash)                              │
│  ├── File System Hierarchy & Permissions                             │
│  ├── Process Management & Signals                                    │
│  ├── Networking Basics (TCP/IP, SSH, NFS, TFTP)                     │
│  └── Package Management & Text Processing (sed, awk, grep)          │
│                                                                      │
│  Phase 2: Toolchains & Cross-Compilation                             │
│  ├── Native vs Cross-Compilation                                     │
│  ├── GNU Toolchain (gcc, binutils, glibc/musl)                      │
│  ├── Crosstool-NG                                                    │
│  ├── Makefiles & CMake for Cross-Compilation                        │
│  └── Sysroot & Staging Concepts                                     │
│                                                                      │
│  Phase 3: Bootloaders (U-Boot)                                       │
│  ├── Boot Process (ROM → SPL → U-Boot → Kernel)                    │
│  ├── U-Boot Configuration & Compilation                              │
│  ├── U-Boot Commands & Environment Variables                         │
│  ├── Device Tree Basics                                              │
│  └── TFTP / NFS Boot                                                 │
│                                                                      │
│  Phase 4: Linux Kernel                                                │
│  ├── Kernel Architecture & Source Tree                                │
│  ├── Kernel Configuration (menuconfig, defconfig)                    │
│  ├── Kernel Compilation & Cross-Compilation                          │
│  ├── Device Tree (DTS/DTB) In-Depth                                 │
│  ├── Kernel Modules (insmod, modprobe, lsmod)                       │
│  └── Kernel Boot Parameters                                         │
│                                                                      │
│  Phase 5: Root Filesystem                                             │
│  ├── Root FS Structure & Init Systems (SysV, systemd, BusyBox)      │
│  ├── BusyBox: Build & Configure                                     │
│  ├── Shared Libraries & Dynamic Linking                              │
│  ├── initramfs vs. Disk-Based Root FS                                │
│  └── Flash File Systems (JFFS2, UBIFS, SquashFS)                    │
│                                                                      │
│  Phase 6: Build Systems                                               │
│  ├── Buildroot (menuconfig, packages, overlays)                      │
│  ├── Yocto Project (BitBake, recipes, layers, BSPs)                 │
│  ├── OpenWRT (for networking devices)                                │
│  └── Comparison & When to Use Which                                  │
│                                                                      │
│  Phase 7: Device Drivers                                              │
│  ├── Character Device Drivers                                        │
│  ├── Platform Drivers & Device Model                                 │
│  ├── I2C, SPI, UART Subsystems                                      │
│  ├── GPIO & Interrupt Handling                                       │
│  ├── DMA & Memory-Mapped I/O                                        │
│  └── Device Tree Bindings for Drivers                                │
│                                                                      │
│  Phase 8: Application Development                                     │
│  ├── POSIX APIs (pthreads, IPC, signals)                             │
│  ├── Socket Programming                                              │
│  ├── D-Bus & Inter-Process Communication                             │
│  ├── File I/O & Memory Management                                    │
│  └── System Programming (fork, exec, mmap)                           │
│                                                                      │
│  Phase 9: Debugging & Profiling                                       │
│  ├── GDB & gdbserver (Remote Debugging)                              │
│  ├── strace, ltrace, ldd                                             │
│  ├── ftrace, perf, eBPF                                              │
│  ├── Kernel Debugging (KGDB, printk, dynamic debug)                 │
│  └── Valgrind & AddressSanitizer                                    │
│                                                                      │
│  Phase 10: Advanced Topics                                            │
│  ├── Real-Time Linux (PREEMPT_RT)                                    │
│  ├── Security (SELinux, AppArmor, Secure Boot)                       │
│  ├── OTA Updates (Mender, RAUC, SWUpdate)                            │
│  ├── Containerization (Docker on Embedded)                           │
│  ├── Embedded Linux Graphics (Wayland, DRM/KMS)                     │
│  └── Embedded Linux Networking (Bridge, VLAN, netfilter)             │
│                                                                      │
└──────────────────────────────────────────────────────────────────────┘
```

### Phase 0: Prerequisites

Before diving into Embedded Linux, make sure you have solid foundations:

| Topic | What to Learn | Resources |
|-------|--------------|-----------|
| **C Programming** | Pointers, structures, memory allocation, bitwise operations, function pointers, linked lists | *The C Programming Language* (K&R), *C Programming: A Modern Approach* (K.N. King) |
| **Computer Architecture** | CPU architecture, memory hierarchy, registers, buses, interrupts, DMA | *Computer Organization and Design* (Patterson & Hennessy) |
| **Git & Version Control** | Branching, merging, rebasing, submodules, patch workflows | [Pro Git Book (free)](https://git-scm.com/book) |
| **Basic Electronics** | Voltage, current, GPIO, pull-up/pull-down, logic levels, UART/SPI/I2C basics | *The Art of Electronics* (Horowitz & Hill) |

### Phase 1: Linux Fundamentals

| Topic | Resources |
|-------|-----------|
| Linux CLI Mastery | [Bootlin Command Line Tutorial (free slides)](https://bootlin.com/blog/command-line/), [Linux Journey](https://linuxjourney.com/) |
| Shell Scripting | [Bash Guide for Beginners](https://tldp.org/LDP/Bash-Beginners-Guide/html/), [Advanced Bash Scripting Guide](https://tldp.org/LDP/abs/html/) |
| Linux System Administration | *The Linux Command Line* by William Shotts [(free PDF)](https://linuxcommand.org/tlcl.php) |
| Linux Internals | *How Linux Works* by Brian Ward |
| System Calls & Programming | *The Linux Programming Interface* by Michael Kerrisk |

### Phase 2: Toolchains & Cross-Compilation

| Topic | Resources |
|-------|-----------|
| Cross-Compilation Concepts | Bootlin Embedded Linux slides (Chapter: Toolchains) |
| Crosstool-NG | [Crosstool-NG Documentation](https://crosstool-ng.github.io/) |
| ARM Toolchains | [ARM GNU Toolchain Downloads](https://developer.arm.com/downloads/-/arm-gnu-toolchain-downloads) |
| Linaro Toolchain | [Linaro Releases](https://releases.linaro.org/components/toolchain/binaries/) |

### Phase 3: Bootloaders (U-Boot)

| Topic | Resources |
|-------|-----------|
| U-Boot Source & Docs | [U-Boot Official](https://u-boot.readthedocs.io/), [U-Boot GitHub](https://github.com/u-boot/u-boot) |
| Boot Process Overview | Bootlin Embedded Linux Training - Bootloader Chapter |
| Device Tree Specification | [devicetree.org](https://www.devicetree.org/specifications/) |
| Practical U-Boot Labs | Bootlin Lab Materials (free) |

### Phase 4: Linux Kernel

| Topic | Resources |
|-------|-----------|
| Kernel Source | [kernel.org](https://www.kernel.org/) |
| Kernel Configuration | `make menuconfig`, `make defconfig` |
| Kernel Internals | *Linux Kernel Development* (Robert Love), *Linux Kernel Programming* (Kaiwan N. Billimoria) |
| Kernel Newbies | [kernelnewbies.org](https://kernelnewbies.org/) |
| Kernel Documentation | [kernel.org/doc](https://www.kernel.org/doc/html/latest/) |

### Phase 5: Root Filesystem

| Topic | Resources |
|-------|-----------|
| BusyBox | [busybox.net](https://busybox.net/) |
| Init Systems | systemd documentation, BusyBox init, SysVinit |
| Flash Filesystems | Kernel docs on JFFS2, UBIFS, SquashFS |
| Building RootFS from Scratch | Bootlin Training Labs |

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

### Phase 7: Device Drivers

| Topic | Resources |
|-------|-----------|
| Linux Device Drivers | *Linux Device Driver Development* (John Madieu), *Linux Device Drivers 3rd Ed* [(free online)](https://lwn.net/Kernel/LDD3/) |
| Kernel Module Programming | [The Linux Kernel Module Programming Guide](https://sysprog21.github.io/lkmpg/) |
| Device Tree for Drivers | [Device Tree Usage](https://elinux.org/Device_Tree_Usage) |

### Phase 8: Application Development

| Topic | Resources |
|-------|-----------|
| POSIX Programming | *The Linux Programming Interface* (Michael Kerrisk) |
| System Programming | *Advanced Programming in the UNIX Environment* (Stevens & Rago) |
| Network Programming | *UNIX Network Programming* (W. Richard Stevens) |
| D-Bus | [D-Bus Tutorial](https://dbus.freedesktop.org/doc/dbus-tutorial.html) |

### Phase 9: Debugging & Profiling

| Tool | Purpose | Reference |
|------|---------|-----------|
| **GDB / gdbserver** | Remote debugging | [GDB Manual](https://sourceware.org/gdb/current/onlinedocs/gdb/) |
| **strace** | System call tracing | `man strace` |
| **ltrace** | Library call tracing | `man ltrace` |
| **ftrace** | Kernel function tracer | [Kernel ftrace docs](https://www.kernel.org/doc/html/latest/trace/ftrace.html) |
| **perf** | Performance analysis | [perf wiki](https://perf.wiki.kernel.org/) |
| **eBPF** | Advanced kernel tracing | *Learning eBPF* (Liz Rice) |
| **Valgrind** | Memory leak detection | [valgrind.org](https://valgrind.org/) |
| **KGDB** | Kernel debugger | Kernel KGDB docs |

### Phase 10: Advanced Topics

| Topic | Resources |
|-------|-----------|
| Real-Time Linux (PREEMPT_RT) | [RT Linux Wiki](https://wiki.linuxfoundation.org/realtime/start), Bootlin RT Training Materials |
| Secure Boot & Security | *Embedded Linux Security* guides, [meta-security (Yocto)](https://git.yoctoproject.org/meta-security) |
| OTA Updates | [Mender.io](https://mender.io/), [RAUC](https://rauc.io/), [SWUpdate](https://sbabic.github.io/swupdate/) |
| Embedded Graphics | [Wayland](https://wayland.freedesktop.org/), DRM/KMS subsystem |
| Containerization | [Balena](https://www.balena.io/), Docker on ARM |
| Linux Networking | [Bootlin Networking Training](https://bootlin.com/training/) |

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
| **Linux Kernel Debugging** | Kaiwan N. Billimoria | 🔴 | Kernel debugging techniques |
| **Linux Kernel Programming** (2025) | Thierry Gayet | 🔴 | Kernel architecture with emphasis on device drivers (USB, PCI, networking) |

### Linux System Programming

| Book | Author(s) | Level | Focus |
|------|-----------|-------|-------|
| **The Linux Programming Interface** | Michael Kerrisk | 🟡🔴 | Definitive Linux/UNIX system programming (1500+ pages) |
| **System Programming in Linux** (2025) | Stewart N. Weiss | 🟡🔴 | Hands-on system programming |
| **Advanced Programming in the UNIX Environment** | Stevens & Rago | 🔴 | UNIX system programming classic |
| **Linux System Programming** | Robert Love | 🟡 | System calls, process management, I/O |

### eBPF & Observability

| Book | Author(s) | Level | Focus |
|------|-----------|-------|-------|
| **Learning eBPF** | Liz Rice | 🟡🔴 | eBPF for observability, networking, security |
| **BPF Performance Tools** | Brendan Gregg | 🔴 | Advanced eBPF performance analysis |

### Bootloader & Build Systems

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
| [**Low Byte Productions**](https://www.youtube.com/@LowByteProductions) | YouTube | Low-level Linux, OS concepts |
| [**FastBit Embedded Brain Academy**](https://www.youtube.com/@FastbitEmbeddedBrainAcademy) | YouTube | Embedded C, MCU, RTOS, Linux |
| [**Wee-W Stack**](https://www.youtube.com/@WeeWStack) | YouTube | Embedded systems concepts |
| [**LiveOverflow**](https://www.youtube.com/@LiveOverflow) | YouTube | Linux security, exploitation, reverse engineering |
| [**Chris Simmonds — Inner Penguin**](https://www.youtube.com/@innerpenguin) | YouTube | Embedded Linux talks and tutorials |

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
| [**Bootlin Training Materials (GitHub)**](https://github.com/bootlin/training-materials) | Bootlin | All training source (LaTeX, CC-BY-SA license) |
| [**Embedded Linux Wiki (eLinux)**](https://elinux.org/) | Community | Massive wiki for embedded Linux |
| [**Linux Kernel Newbies**](https://kernelnewbies.org/) | Community | Beginner-friendly kernel resources |
| [**The Linux Documentation Project**](https://tldp.org/) | Community | HOWTOs, guides, FAQs |
| [**ARM Education Embedded Linux Kit**](https://www.arm.com/resources/education/education-kits/embedded-linux) | ARM | Embedded Linux education kit |
| [**Linux From Scratch (LFS)**](https://www.linuxfromscratch.org/) | Community | Build entire Linux system from source |

---

## 💰 Online Courses (Paid)

| Course | Platform | Instructor / Provider |
|--------|----------|-----------------------|
| [Embedded Linux Step by Step Using Beaglebone Black](https://www.udemy.com/course/embedded-linux-step-by-step-using-beaglebone/) | Udemy | FastBit EBA (Kiran Nayak) |
| [Linux Device Driver Programming Using Beaglebone Black](https://www.udemy.com/course/linux-device-driver-programming-using-beaglebone-black/) | Udemy | FastBit EBA |
| [Embedded Linux](https://www.udemy.com/course/embedded-linux/) | Udemy | Israel Gbati |
| [Embedded Linux Development (LFD450)](https://training.linuxfoundation.org/training/embedded-linux-development/) | Linux Foundation | Linux Foundation |
| [Introduction to Linux (LFS101x)](https://www.edx.org/learn/linux/the-linux-foundation-introduction-to-linux) | edX | Linux Foundation (FREE) |
| [Embedded Linux with QEMU Workshop](https://embeddedonlineconference.com/session/Using_QEMU_to_Get_Started_with_Embedded_Linux) | EOC | Mohammed Billoo |

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
| **BeagleBone Black** | TI AM335x (ARM Cortex-A8) | ~$55 | Classic embedded Linux learning |
| **BeaglePlay** | TI AM6254 (ARM Cortex-A53) | ~$30 | Modern, affordable, great community |
| **Raspberry Pi 4/5** | Broadcom (ARM Cortex-A72/A76) | ~$35-$80 | Versatile, massive community |
| **STM32MP157 Discovery** | STM32MP157 (Cortex-A7 + M4) | ~$70 | Dual-core (Linux + RTOS), industrial |
| **STM32MP2 Discovery** | STM32MP2 (Cortex-A35 + M33) | ~$99 | Latest ST platform |
| **NXP i.MX93 EVK** | NXP i.MX93 (Cortex-A55 + M33) | ~$100+ | NXP ecosystem, Yocto support |
| **NVIDIA Jetson Nano** | Tegra X1 (ARM Cortex-A57) | ~$150 | AI/ML at the edge + Linux |
| **Pine64 / Rock64** | Rockchip (ARM) | ~$25-$45 | Budget-friendly ARM boards |
| **RISC-V Boards** (VisionFive 2, Milk-V) | RISC-V | ~$40-$100 | Emerging architecture |

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
| **Binwalk** | Firmware analysis & extraction |
| **minicom / picocom** | Serial terminal communication |
| **OpenOCD** | On-chip debugging via JTAG/SWD |
| **devmem2** | Direct memory access from userspace |
| **i2c-tools** | I2C bus utilities |
| **spidev-tools** | SPI testing utilities |
| **mtd-utils** | Flash memory management |
| **Mender / RAUC / SWUpdate** | OTA update frameworks |

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
| [**Embitude**](https://embitude.in/) | Embedded Linux training & roadmaps (India) |
| [**Sergey Mironov**](https://sergeev.io) | Linux kernel & embedded blog |
| [**2net.co.uk (Chris Simmonds)**](https://2net.co.uk/) | Inner Penguin - Embedded Linux blog |
| [**Embedded Related**](https://www.embeddedrelated.com/) | Embedded systems articles & forums |
| [**Nathan Jones Blog**](https://www.embeddedrelated.com/showarticle/1589.php) | Embedded systems roadmaps & curricula |
| [**Yocto Project Blog**](https://www.yoctoproject.org/blog/) | Official Yocto news and tutorials |
| [**Linux Kernel Mailing List Archives**](https://lkml.org/) | Kernel development discussions |

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
  <a href="https://embeddexai.com">EmbeddexAI</a> | <a href="https://github.com/eslamnasr">GitHub</a> | <a href="https://linkedin.com/in/eslamnasr">LinkedIn</a>
</p>
