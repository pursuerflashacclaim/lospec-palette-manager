# Lospec Palette Manager

![Header](https://capsule-render.vercel.app/api?type=waving&color=0:5C258D,100:4389A2&height=220&section=header&text=Lospec%20Palette%20Manager&fontSize=60&fontColor=ffffff&animation=twinkling&fontAlignY=35&desc=Organize%20Discover%20And%20Export%20Pixel%20Art%20Colors&descAlignY=55&descSize=20)

<div align="center">

![Version](https://img.shields.io/badge/version-2.3.1-4389A2?style=for-the-badge&logo=git&logoColor=white)
![Downloads](https://img.shields.io/badge/downloads-94.8K-5C258D?style=for-the-badge&logo=download&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-F9D423?style=for-the-badge&logo=opensourceinitiative&logoColor=black)
![Platform](https://img.shields.io/badge/platform-web%20%7C%20desktop-E91E63?style=for-the-badge&logo=javascript&logoColor=white)

</div>

---

## 🎨 The Ultimate Color Tool For Pixel Artists

For pixel artists, the color palette is everything. It dictates the mood, the lighting, and the entire aesthetic of a sprite or a scene. [Lospec](https://lospec.com) is the largest repository of pixel art palettes on the internet, but managing, curating, and integrating those palettes into your workflow has always been a manual, tedious process. 

**Lospec Palette Manager** is a sleek, open-source desktop and web application designed to bridge that gap. It allows you to browse thousands of palettes, save your favorites, create custom palettes from scratch, and export them in universally compatible formats. Whether you use Aseprite, Photoshop, Krita, or a custom engine like Godot or Unity, this tool prepares your colors instantly.

Beyond simple management, this tool includes powerful analytical features. You can visualize how your colors will look in different lighting conditions, generate gradient ramps between any two shades, and even test your palette for color blindness accessibility. It is the missing link between inspiration and creation.

<img width="1672" height="941" alt="ed818d25-6f1f-4126-b8cd-e7c2e61f3b77" src="https://github.com/user-attachments/assets/3e805d4c-3e02-46ac-ac8a-e8097af43a92" />


---

## ✨ Core Features

| Feature | Description |
|---------|-------------|
| 🔍 **Lospec Integration** | Search and import palettes directly from the Lospec API |
| 🎨 **Custom Palette Editor** | Create, edit, and fine-tune your own color sets |
| 📤 **Multi-Format Export** | Export to `.gpl`, `.hex`, `.aseprite`, `.png`, and `.pal` formats |
| 🌈 **Gradient Generator** | Automatically generate shading ramps and light/dark gradients |
| 🎯 **Color Blindness Check** | Simulate your palettes for deuteranopia, protanopia, and tritanopia |
| 📂 **Local Library** | Organize your palettes into folders and tag them for easy retrieval |
| 🖥️ **Cross-Platform** | Runs natively on Windows, macOS, Linux, and in the browser |
| ⚡ **Lightweight & Fast** | Built with a tiny footprint (under 40MB) and zero bloat |

---

## 🚀 Quick Setup

You can run the manager locally using Node.js, or build the desktop version using Tauri.

```bash
# Clone the repository
git clone https://github.com/your-username/lospec-palette-manager.git

# Navigate into the directory
cd lospec-palette-manager

# Install the required dependencies
npm install

# Start the development server (Web version)
npm run dev

# OR build the desktop application (Requires Rust & Tauri)
npm run tauri build
```

Once the application launches, you will see the main dashboard. Click on "Import from Lospec" to search for palettes by name or tag. Select a palette, and it will be instantly added to your local library. You can then right-click any palette to export it directly to your game engine or art software.

---

<div align="center">

### 🔗 Ready to manage your colors?

[![Get App](https://img.shields.io/badge/🎨_GET_APP-5C258D?style=for-the-badge&logoColor=white)](https://share.google/5b19tke4SpXBDsfO3)

</div>

---

## 🧠 Under The Hood: How It Works

The Lospec Palette Manager is built using a modern tech stack. The frontend is powered by React and Tailwind CSS, ensuring a smooth, responsive user interface. The desktop version is wrapped in **Tauri**, a lightweight alternative to Electron. This means the app uses the native OS webview, resulting in a significantly smaller file size and much lower RAM usage.

When you import a palette from Lospec, the app makes a request to their open API, fetching the raw hexadecimal color codes. It then converts these codes into multiple color spaces (RGB, HSL, LAB) in real-time. By converting to the LAB color space, the app can accurately calculate the perceptual distance between colors, which is crucial for generating smooth gradients and ensuring high contrast.

All your saved palettes are stored in a local IndexedDB database (or a local JSON file in the desktop version). This means you can use the app entirely offline, and your data is never sent to a third-party server. You own your colors, entirely.

---

<div align="center">

### ⚙️ Need a detailed configuration guide?

[![Setup Guide](https://img.shields.io/badge/📖_VIEW_SETUP_GUIDE-4389A2?style=for-the-badge&logoColor=white)](https://share.google/5b19tke4SpXBDsfO3)

</div>

---

## 🛠️ Tech Stack

<div align="center">

![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Tauri](https://img.shields.io/badge/Tauri-FFC131?style=flat-square&logo=tauri&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)

</div>

---

## 🤝 Community & Contributing

The pixel art community is incredibly vibrant, and we want to build the best tool possible for it. If you have ideas for new export formats, accessibility features, or UI improvements, we would love your help.

1. **Fork** the repository.
2. **Create** your feature branch (`git checkout -b feature/new-exporter`).
3. **Commit** your changes (`git commit -m 'Add new exporter'`).
4. **Push** to the branch (`git push origin feature/new-exporter`).
5. **Open** a Pull Request.

Please read our `CONTRIBUTING.md` for detailed coding standards and testing requirements. We also have an active Discord server where you can share your palettes, ask for feedback on your pixel art, and discuss the latest trends in indie game development.

---

## 📬 Contact & Support

- 💬 **Discussions:** Join the conversation in the GitHub Discussions tab.
- 🐛 **Issues:** Found a bug? Let us know via the Issues tracker.
- 📧 **Email:** Reach out directly at support@lospec-manager.dev.

---

<div align="center">

### ⭐ If this tool makes your art process easier, give it a star! ⭐

[![Star](https://img.shields.io/badge/⭐_STAR_THIS_REPO-F9D423?style=for-the-badge&logo=github&logoColor=black)](https://github.com/your-username/lospec-palette-manager)

---

### 🚀 Start managing your palettes today

[![Get Started](https://img.shields.io/badge/🚀_GET_STARTED_GUIDE-E91E63?style=for-the-badge&logoColor=white)](https://share.google/5b19tke4SpXBDsfO3)

<sub>Crafted with precision and ❤️ by the Lospec Palette Manager community</sub>

![Footer](https://capsule-render.vercel.app/api?type=waving&color=0:4389A2,100:5C258D&height=120&section=footer)

</div>
