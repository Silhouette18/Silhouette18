
# Hi, I'm Svyatoslav Nikolenko

### Linux Systems Developer | C | Rust | Linux Kernel

I am a systems programmer interested in Linux kernel development, low-level debugging, networking, and filesystem internals.

I work primarily with **C** and **Rust**. My hands-on experience includes developing Linux kernel modules, investigating kernel bugs reported by syzbot, debugging driver issues, and submitting patches to the Linux kernel community.

My main areas of interest are **Linux Memory Management (MM), VFS, kernel internals, and networking**.

## Technical Skills

- **Languages:** C, Rust, Python, Bash, Assembly
- **Linux systems:** Kernel modules, driver debugging, Linux internals, kernel build and debugging workflows
- **Kernel development:** syzbot bug investigation, patch submission, upstream review process
- **Networking:** IPv4, TCP, UDP, ICMP, Linux TUN (`/dev/net/tun`)
- **Tools:** Git
- **Additional familiarity:** Docker, Kubernetes

## Selected Projects

### [Linux RAMFS](https://github.com/Silhouette18/linux-ramfs)

An experimental in-memory filesystem implemented in **C** as an out-of-tree Linux kernel module. The project works with Linux VFS interfaces and implements filesystem functionality such as mounting and file operations.

### [Rust TUN Networking](https://github.com/Silhouette18/rust-tun-networking)

An experimental **Rust** user-space networking project built around Linux `TUN` (`/dev/net/tun`). It processes IPv4 traffic, handles ICMP, UDP, and TCP flows, and relays traffic through regular operating-system sockets.

## Linux Kernel Contributions

I have submitted patches across several Linux kernel subsystems, investigated syzbot-reported issues, and participated in upstream review discussions.

### Staging

**`staging: vme_user: Use str_enabled_disabled() helper`**

- Included in Greg Kroah-Hartman's `staging-7.4-rc1` pull request.
- [Staging 7.4-rc1 pull request](https://lore.kernel.org/all/atoUedBI3u813dYW@kroah.com/)

**`staging: rtl8723bs: Remove manual ifname allocation`**

- Iterated through multiple review revisions (v1–v6).
- Included in Greg Kroah-Hartman's `staging-7.4-rc1` pull request.
- The driver was subsequently removed through the Wi-Fi driver tree, superseding this cleanup in the final mainline history.
- [Staging 7.4-rc1 pull request](https://lore.kernel.org/all/atoUedBI3u813dYW@kroah.com/)

### Media

**`media: usbtv: fix use-after-free and lockdep panic on unbind`**

- Investigated a syzbot-reported use-after-free and lockdep panic in the USBTV driver.
- Analyzed device lifetime, reference counting, and USB driver teardown.
- Patch committed by Hans Verkuil in the media subsystem tree.
- [Patch discussion on lore.kernel.org](https://lore.kernel.org/all/20260930100000.41652-1-nsvatoslav515@gmail.com/)

### Networking

**`net: e1000: fix warning in iounmap on probe failure`**

- Investigated a syzbot-reported warning in the Intel e1000 driver's probe error path.
- Received `Reviewed-by` from Aleksandr Loktionov.
- Applied by Tony Nguyen to the `net-queue` development tree and subsequently included in the `1GbE` integration series.
- [Patch in the netdev integration series](https://lore.kernel.org/all/20261113005823.130021-4-anthony.l.nguyen@intel.com/)

## Current Interests

- Linux Memory Management (MM)
- Virtual File System (VFS)
- Page cache and filesystem/kernel interactions
- Linux networking and kernel debugging

---

I enjoy investigating low-level problems, understanding their root causes, and developing focused fixes.
<!--
**Silhouette18/Silhouette18** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
