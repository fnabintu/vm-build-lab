# VM Build Lab

A free, interactive lab that teaches beginners what a virtual machine is, how it works under the hood, and how to build their own Kali Linux VM on **Windows, macOS (Intel or Apple Silicon), or Linux**.

**▶ Try it live:** [fnabintu.github.io/vm-build-lab](https://fnabintu.github.io/vm-build-lab/)

Built by Felista Nabintu for the Women in CyberSecurity (WiCyS) student chapter at the University of Arizona.

## What's inside

The lab has 10 hands-on stations. Students pick their computer once, and every step adapts to it with the right downloads, commands, and menu names.

| Station | What students do |
|---|---|
| What is a VM? | Explore the virtualization stack layer by layer |
| How it works inside | Five tabs on CPU (VT-x / AMD-V, VM exits), memory (EPT / NPT), storage (`.vmdk`, thin provisioning, snapshot deltas), networking (NAT / Bridged / Host-only), and devices (paravirtualization, VM escape) |
| Why use one? | Scenario questions on sandboxing and legal, ethical practice |
| Know your computer | Identify their OS and chip, check virtualization support, get their download kit |
| 1 · Install VMware | Install Workstation Pro or Fusion (free for personal use) |
| 2 · Download & check Kali | Download zSecurity's custom Kali build and verify its SHA256 hash in a simulated terminal |
| 3 · Unzip & open | Extract the `.7z` and open the `.vmx` (or `.vmwarevm` on Apple Silicon) |
| 4 · Choose settings | Allocate RAM and CPU and pick a network mode, with feedback on mistakes |
| 5 · Change the password | Replace the default `root` / `toor` login with `passwd` |
| 6 · Snapshot = undo | Take a snapshot, break the VM, and restore it |

Every station ends with a one-line takeaway, and the last screen is a cheat sheet for the student's own computer.

### Features

- Plain-language explanations side by side with the technical details
- OS-specific instructions for Windows, Intel Mac, Apple Silicon Mac, and Linux
- Light and dark modes
- Progress saved in the browser, so students can come back later
- Works on phones, tablets, and laptops
- Plain HTML, CSS, and JavaScript in a single file, with no frameworks and no build step

## Run it

Open `index.html` in any modern browser. That's it.

### Publish it with GitHub Pages

1. In this repository, go to **Settings › Pages**.
2. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
3. Choose the `main` branch and the `/ (root)` folder, then click **Save**.
4. After a minute or two, the lab is live at `https://fnabintu.github.io/vm-build-lab/`.

## Keeping it up to date

zSecurity updates its Kali builds over time. The direct download links and SHA256 hashes live in the `OS`, `KX64`, and `KARM` objects near the top of the script in `index.html`. When a new build comes out, update the links and hashes from the [zSecurity Download Custom Kali page](https://zsecurity.org/download-custom-kali/). Every download section in the lab also links to that page as a fallback.

## Ethics

Kali Linux contains real security tools. Only test systems you own or have written permission to test. The lab teaches students to keep their VM on NAT networking and to practice on machines they built themselves.

## Credits

- Custom Kali Linux builds by [zSecurity](https://zsecurity.org/download-custom-kali/)
- [Kali Linux](https://www.kali.org/) by OffSec
- [VMware Workstation Pro and Fusion](https://support.broadcom.com/) by Broadcom
- [7-Zip](https://www.7-zip.org/) by Igor Pavlov
- WiCyS University of Arizona Student Chapter

This project is not affiliated with or endorsed by zSecurity, OffSec, or Broadcom.

## License

The code is released under the [MIT License](LICENSE). The WiCyS chapter logo belongs to the WiCyS University of Arizona Student Chapter and is not covered by the MIT License.
