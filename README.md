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
