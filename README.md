### **mpvs (Minimal Player Video Summoner)**

> *“Summon a single mpv instance—no clutter, no duplicates.”*
---
### **📝 GitHub Project Description (README excerpt)**
**mpvs** is a lightweight wrapper script for `mpv` that enforces **single-instance playback** using its IPC mechanism. When you open a video, it sends it to the same mpv window — no duplicates, no mess.

---

### 🔧 Features

* 🧠 **Single window**: All files play in the same persistent mpv session
* 🧼 **Simple IPC**: No background daemons or bloated frontends
* 🧩 **Fully compatible** with your `mpv.conf`, keybindings, and scripts
* 🧪 **Failsafe**: Auto-recovers from stale sockets or crashed sessions
* 📦 **.deb installer** for system-wide installation

---

### 🚀 Installation

```bash
sudo dpkg -i mpvs.deb
```

---

### 📄 Usage
Mainly for GUI. just chose MPVS as default video and audio luncher.
it will also work on commandline if you like that spceailly if you use CLI file manager.

```bash
mpvs video1.mp4
mpvs video2.webm
```

Both play in the same window. If mpv isn’t running, it will start.

---

### 🛠 Dependencies

* `mpv` (>= 0.29)
* `socat`

---

### 📁 Files Installed

* `/usr/local/bin/mpvs` – the main script
* `/usr/share/applications/mpvs.desktop` – launcher entry
---
### Build
```
git clone https://github.com/amyrkmal/MPVS.git
cd mpvs
dpkg-deb --build --root-owner-group ./ mpvs.deb 

```
