# 📋 REPORT: Laboratory Work №1
**Course:** Operating Systems  
**Topic:** Introduction to the Virtual Machine Environment and Features of the Linux Operating System  
**Institution:** KYIV VOCATIONAL COLLEGE OF COMMUNICATION

---

## 👤 Student Information
* **Student:** Ruda Daryna Serhiivna
* **Group:** BIKS-33
* **Teacher:** Sushanova Viktoriia Serhiivna
* **Year:** 2026

---

## 🎯 Objectives
1. Familiarization with different types of hypervisors and virtualization in OS.
2. Overview of modern operating systems and their capabilities.

---

## 📚 1. Preliminary Preparation

### 🔡 Basic English Glossary
```yaml
- Virtual Machine (VM): Software emulation of a physical computer.
- Virtualization: Technology for creating virtual computing resources.
- Hypervisor: Software that manages VMs.
- Type 1 (Bare-metal): Runs directly on hardware (e.g., Hyper-V, ESXi).
- Type 2 (Hosted): Runs on top of a host OS (e.g., VirtualBox, VMware Player).
- Host/Guest OS: The main system vs. the system inside the VM.
⚙️ Hypervisor Types & Hyper-V (Variant 15)Hypervisor is specialized software for managing virtual machines.Hyper-V Components:Parent Partition: Management environment (Windows).Child Partitions: Where Guest OSs live.Virtual Switch: Networking for VMs.VHD/VHDX: Virtual disk formats.🛠 2. Execution Procedure2.1 Deployment Steps (VirtualBox)Install Oracle VirtualBox.Download Linux ISO (e.g., Ubuntu).Create VM (Allocate RAM & CPU).Create Virtual Hard Disk.Attach ISO and launch the installer.Complete OS setup & install Guest Additions.2.2 Hardware LimitationsFeature32-bit OS64-bit OSRAM SupportMax ~4 GB> 4 GB (Huge limits)CPU RequirementAny modern CPU64-bit CPU onlyVirtualizationSoftware onlyRequires Intel VT-x / AMD-V2.3 Installing GNOME/KDE (via Terminal)If you are in CLI mode, use these commands to install a GUI:Bash# Update repositories
sudo apt update

# Install GNOME
sudo apt install gnome-shell gnome-session gnome-terminal

# Install KDE Plasma
sudo apt install kde-standard # Or kde-full for everything
🖥️ 2.4 Graphical Interfaces (Variant 15)Xfce: Lightweight, stable, and fast. Perfect for low-end hardware.FVWM: Extremely flexible window manager for advanced users. Minimalist and fast.❓ 3. Control Questions⚖️ Type 1 vs Type 2 HypervisorsType 1: Higher performance, used in Servers/Clouds.Type 2: Easier to use, used for Desktop testing/Learning.📜 GNU GPL ConceptThe General Public License ensures 4 freedoms:Run the program.Study the code.Modify the code.Redistribute (Original or Modified).🤖 Android & Linux RelationshipAndroid uses the Linux Kernel for core hardware management (drivers, memory, process control) but has its own UI and runtime (ART).⌨️ Changing Boot Mode (CLI vs GUI)Bash# Switch to Text Mode (Multi-user)
sudo systemctl set-default multi-user.target

# Switch to Graphical Mode
sudo systemctl set-default graphical.target
✅ ConclusionIn this lab, I explored virtualization principles and the Linux ecosystem. I learned the difference between Type 1 and Type 2 hypervisors, studied the Hyper-V architecture, and practiced the deployment process in VirtualBox. Understanding open-source licensing (GPL) and the variety of Desktop Environments (Xfce, KDE) provides a solid foundation for further Linux system administration.
