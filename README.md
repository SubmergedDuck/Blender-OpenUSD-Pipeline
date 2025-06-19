# Blender to OpenUSD Pipeline Demo
This project demonstrates a working pipeline to export 3D content from **Blender** into **OpenUSD (Universal Scene Description)** format, preserving geometry, animation, and scene hierarchy. It showcases a foundational understanding of USD-based workflows for real-time graphics, virtual production, and asset management.

---

## 📦 Project Structure

```plaintext
usd-pipeline-demo/
├── blender_scene.blend            # Original scene in Blender
├── exports/
│   ├── scene.usda                 # Main composed USD scene
│   ├── character.usda             # Character geometry and animation
│   ├── environment.usda           # Static environment assets
│   └── materials.usda             # Material definitions
├── scripts/
│   └── inspect_scene.py           # Python script to inspect USD data
├── screenshots/
│   ├── blender_viewport.png
│   └── usdview_hierarchy.png
├── README.md
```

## 🛠 Tools Used

- [Blender](https://www.blender.org/) (vX.X) with USD Export Add-on
- [Pixar USD SDK](https://github.com/PixarAnimationStudios/USD)
- `usdview` for USD visualization
- Python 3.9+ for scene inspection
- *(WIP)* NVIDIA Omniverse Create for layered scene review

---

## ✅ Features Demonstrated

- ✅ Exporting mesh, materials, and animation from Blender to USD
- ✅ Scene composition using multiple `.usda` files (character, environment, lighting)
- ✅ Layered hierarchy and references
- ✅ Python script to parse and inspect USD scene structure
- ✅ Visual comparison between Blender and USD representations

---

## 🧪 How to Run

1. Clone this repo
2. Open `blender_scene.blend` and export the scene as `.usda` using the USD add-on
3. Run:
   ```bash
   usdview exports/scene.usda
   ```
4. Run the Python script:
   ```bash
   python3 scripts/inspect_scene.py
   ```

---

## 🧠 What I Learned

- How OpenUSD represents a 3D scene using **prims**, **layers**, and **composition arcs**
- How to structure modular scene exports (character/environment separation)
- How to inspect and manipulate a USD file with the **Python API**
- Importance of real-time asset pipelines and scenegraph architecture

---

## 📸 Screenshots

| Blender Viewport                | USDView Scene Hierarchy           |
|--------------------------------|-----------------------------------|
| ![](screenshots/blender_viewport.png) | ![](screenshots/usdview_hierarchy.png) |

---

## 🚀 Future Improvements

- Add lighting variants (e.g., day/night)
- Implement shader/material translation
- Integrate with Omniverse Create for more advanced previews
- Live-edit with Python and auto-reload in viewer

---

## 💬 Contact

Made by [SubmergedDuck](https://github.com/submergedduck)
