# 🛠️ TeckyUI - System Toolkit Overlay

TeckyUI is a powerful Windows overlay application built using **C++**, **Dear ImGui**, and **DirectX 11**. It provides real-time access to system tools including process management, terminal command execution, internet control, system cleanup, and performance monitoring — all within a slick, interactive UI overlay.

> Developed with purpose and precision by **Khawar Ahemad Khan**.

---

## ✨ Features

### 🧩 Modular Tool Tabs
- **Settings**
  - Self-hide and stream-safe window.
  - Hotkey toggles (`F9` to show/hide UI, `F10` to exit).

- **Terminal**
  - Execute any system command.
  - Displays full output and exit codes.
  - Scrollable command/output history.

- **Process Manager**
  - Live process listing with search and filtering.
  - Kill processes by selection.

- **Internet Control**
  - Block/resume internet access using Windows Firewall.
  - Visual status indicator.

- **System Cleaner**
  - Deletes system and user temporary files.
  - Flushes DNS and resets critical folders.
  - Terminal clear function included.

- **FPS Counter**
  - Non-intrusive real-time FPS overlay at the top-left.

---

## 🧪 Technology Stack

| Layer         | Technology         |
|---------------|--------------------|
| UI Rendering  | Dear ImGui         |
| Graphics API  | DirectX 11         |
| System Access | WinAPI             |
| Styling       | Custom ImGui Theme |
| OS Support    | Windows 10/11      |

---

## 📸 Stream-Safe Design

TeckyUI uses `SetWindowDisplayAffinity` to avoid screen capturing by OBS or screen recorders. This ensures sensitive tools stay hidden during streams or screen shares.

---

## 🔐 Requirements

- Windows 10 or 11 (64-bit)
- Administrator privileges (for full feature access)
- GPU that supports DirectX 11
---

## 🧱 Build Instructions

### 📦 Dependencies
- Visual Studio 2019+ with Windows Desktop Development workload
- Dear ImGui (included or submodule)
- Link against:
  - `d3d11.lib`
  - `dwmapi.lib`
  - `wininet.lib`
  - `psapi.lib`

### 🧰 Compilation
```bash
git clone https://github.com/your-repo/TeckyUI.git
cd TeckyUI
```
# Open the solution in Visual Studio and build in Release x64


---

### 🧾 **Part 4: License, Developer, and Plans**

---

## ⚠️ Disclaimer

This tool performs administrative tasks such as terminating processes and modifying firewall settings. Use responsibly.

---

## 👨‍💻 Developer

**Khawar Ahemad Khan**  
Engineering mindset. Focused on building smart, efficient, and forward-thinking system tools.

---

## 📃 License

📄 [MIT License](https://github.com/khawarahemad/HIDE-S?tab=MIT-1-ov-file#)

---

## 🚀 Future Plans

- Threaded command execution
- Per-process network control
- Modern WFP-based internet blocking
- Dynamic system metrics (CPU/GPU/RAM)
- ImGui Docking support for modular layout

---
## 🤝 Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes.

---

## 🐞 Known Issues

- Internet control may require Windows Firewall to be enabled  
- Some system cleaner operations might fail if files are in use  
- Process killing may not work for protected system processes  
---

> _“A tool is only as powerful as the clarity of its interface.” — TeckyUI Philosophy_


