# 🧩 IMG Mounter

A lightweight **Bash-based image mounting utility** for Linux that provides both a **Graphical (Zenity)** and **Terminal (Whiptail)** interface.

Easily mount and unmount `.img` files with just a few clicks — no commands needed!  

---

## ✨ Features

✅ Mount and unmount `.img` files (supports multiple partitions)  
✅ Dual interface: **GUI (Zenity)** and **TUI (Whiptail)**  
✅ Read-only or Read & Write mount modes  
✅ Simple install and uninstall

---

## 📦 Installation

Run the following commands in your terminal:

```bash
# Download the script
wget https://raw.githubusercontent.com/vihatsoft/img-mounter/main/imgmount -O imgmount

# Make it executable
chmod +x imgmount

# Install system-wide (requires sudo)
sudo ./imgmount install
```

After installation:
- Run command : `sudo imgmount`

---

## 🚀 Usage

### 🖥️ **Open GUI or TUI Mode**

- run this in terminal choose GUI or TUI mode:
  ```bash
  sudo imgmount
  ```

The GUI lets you:
- Mount `.img` files (read-only or writable)
- Unmount mounted images

---

## 🔧 Uninstallation

To completely remove IMG Mounter:

```bash
sudo rm -f /usr/local/bin/imgmount
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
| Install | `sudo ./imgmount install` |
| Launch GUI/TUI | `sudo imgmount` → Choose option 1 |
| Uninstall | Run from menu → “Uninstall” or manually remove files |

---

Enjoy simple and safe `.img` mounting! 🚀
