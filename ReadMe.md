# 🧩 IMG Mounter

A lightweight **Bash-based image mounting utility** for Linux that provides both a **Graphical (Zenity)** and **Terminal (Whiptail)** interface.

Easily mount and unmount `.img` files (such as Raspberry Pi OS backups, disk images, etc.) with just a few clicks — no commands needed!  

---

## ✨ Features

✅ Mount and unmount `.img` files (supports multiple partitions)  
✅ Dual interface: **GUI (Zenity)** and **TUI (Whiptail)**  
✅ Auto-downloads custom icon for app  
✅ Creates Desktop and Application Menu shortcut  
✅ Read-only or Read & Write mount modes  
✅ Progress dialog during unmounting  
✅ Simple install and uninstall

---

## 📦 Installation

Run the following commands in your terminal:

```bash
# Download the script
wget https://raw.githubusercontent.com/<your-username>/img-mounter/main/imgmount.sh -O imgmount.sh

# Make it executable
chmod +x imgmount.sh

# Install system-wide (requires sudo)
sudo ./imgmount.sh install
```

After installation:
- Command-line tool: `/usr/local/bin/imgmount`
- Icon stored at: `~/.config/imgmount/imgmount_icon.png`
- Desktop shortcut: `~/Desktop/IMG_Mounter.desktop`
- Application menu entry: `Utility → IMG Mounter`

---

## 🚀 Usage

### 🖥️ **Open GUI Mode (Zenity)**

- From your **Desktop shortcut**, double-click “**IMG Mounter**”
- OR run this in terminal:
  ```bash
  imgmount gui
  ```

The GUI lets you:
- Mount `.img` files (read-only or writable)
- Unmount mounted images
- View progress and success dialogs

---

### 💻 **Open Terminal Mode (Whiptail)**

Run the tool without arguments:
```bash
imgmount
```

You’ll see a menu like this:
```
Choose Interface:
  1) Terminal (Whiptail)
  2) GUI (Zenity)
```
Choose **1** for the text-based interface.

---

## 🔧 Uninstallation

To completely remove IMG Mounter:

```bash
sudo rm -f /usr/local/bin/imgmount
rm -rf ~/.config/imgmount
rm -f ~/Desktop/IMG_Mounter.desktop
rm -f ~/.local/share/applications/IMG_Mounter.desktop
```

Or open the app → select **“Uninstall”** from the main menu.

---

## 🧠 Requirements

- Debian / Ubuntu / Raspberry Pi OS  
- `zenity`, `whiptail`, `losetup`, `mount`, `coreutils`, `wget`

If not found, they’ll be installed automatically during setup.

---

## 💡 Quick Summary

| Task | Command / Action |
|------|------------------|
| Install | `sudo ./imgmount.sh install` |
| Launch GUI | `imgmount gui` or click Desktop Icon |
| Launch TUI | `imgmount` → Choose option 1 |
| Uninstall | Run from menu → “Uninstall” or manually remove files |

---

Enjoy simple and safe `.img` mounting! 🚀
