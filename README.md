<img width="1002" height="912" alt="image" src="https://github.com/user-attachments/assets/04c08ec1-a76f-4af3-8774-bc9cc12d4566" />

# 🚗 GTA V Vehicle Photo Catalog

An interactive catalog containing **13,000+ WebP vehicle images** for **490+ GTA V vehicles**, designed for FiveM developers, server owners, and web projects.

This project includes a modern HTML catalog with search, category filtering, color selection, and multiple image resolutions, making it easy to browse and integrate vehicle images into any project.

---

# 🚀 Installation

1. Download the latest release: [**v1.1 (.7z, 165 MB)**](https://github.com/MbarekTR/gta-v-vehicle-photo-catalog/releases/download/v1.1/gta-v-vehicle-photo-catalog-v1.1.7z)
2. Extract the archive (requires [7-Zip](https://www.7-zip.org/) or similar)
3. Open **index.html** in your browser

> ⚠️ **Note:** Some browsers block local image loading due to CORS restrictions when opening `index.html` directly (`file://`). If images don't load, serve the folder with a local server instead, e.g.:
> ```bash
> python -m http.server 8000
> ```
> then visit `http://localhost:8000`

See all releases: [Releases page](https://github.com/MbarekTR/gta-v-vehicle-photo-catalog/releases/tag/v1.0)

---

# ✨ Features

* 🚗 490+ GTA V vehicles
* 🖼️ 13,000+ WebP images
* 🎨 4 color variants
  * Black
  * Blue
  * Red
  * White
* 📐 7 image resolutions
  * Original
  * 512x512
  * 256x256
  * 128x128
  * 64x64
  * 32x32
  * 24x24
* 🔍 Vehicle search
* 📂 Category filtering
* 🌐 Interactive HTML catalog
* 📁 Organized folder structure
* ⚡ Ready to use

---

# 📦 Package Information

| Item            |       Value |
| --------------- | ----------: |
| Vehicles        |    **490+** |
| Images          | **13,000+** |
| Format          |    **WebP** |
| Compressed Size |  **172 MB** |
| Extracted Size  |  **202 MB** |

---

# 💡 Possible Uses

This package can be used in a wide variety of GTA V/FiveM projects, including:

* 🚗 Vehicle dealerships
* 📱 In-game phone applications
* 📋 Vehicle selection menus
* 🎒 Inventory systems
* 🌍 Websites
* 🤖 Discord bots
* 📚 Vehicle databases
* 📖 Documentation
* 🎨 Any custom project

All images use the original **GTA V vehicle spawn names** as filenames, allowing quick and easy integration into scripts, websites, and other applications.

---

# 🧑‍💻 Developer Notes

`vehicles_data.js` gives you the full vehicle list and folder structure programmatically:

```js
{
    "category": "boats",
    "name": "avisa",
    "images": [
        "boats/avisa/avisa_black.webp",
        "boats/avisa/avisa_blue.webp",
        "boats/avisa/avisa_red.webp",
        "boats/avisa/avisa_white.webp"
    ]
}
```

These paths are a lightweight index, not the final file paths. Each real file on disk follows this pattern:

```
<category>/<vehicle>/<color>/<vehicle>_<color>_<size>.webp
```

For example, the `avisa` entry above maps to:

```
boats/avisa/black/avisa_black_original.webp
boats/avisa/black/avisa_black_256x256.webp
boats/avisa/black/avisa_black_128x128.webp
...
```

`<size>` can be `original`, `512`, `256`, `128`, `64`, `32`, or `24` (as `WxH`). `index.html` builds these paths at runtime — see the `normalizeImagePath()` and `getResizedImagePath()` functions if you want to reuse that logic in your own scripts.

---

# 📝 Notes

* This package **does not include every GTA V vehicle**. Some vehicles were excluded because they could not be captured correctly due to camera limitations, model size, or other technical constraints.
* Cars generally have the highest image quality. Larger vehicles such as **boats, helicopters, planes, trains, and some utility vehicles** may have slightly different framing due to their dimensions.
* The included **index.html** provides an interactive catalog where you can:
  * Search vehicles
  * Filter by category
  * Switch between available colors
  * Preview all available image resolutions
* Developers can also use **vehicles_data.js** to access the complete vehicle list and folder structure programmatically.

---

# ⚖️ Disclaimer

This repository is an unofficial fan-made project.

Grand Theft Auto V, its vehicles, names, trademarks, and other related assets are the property of Rockstar Games and/or Take-Two Interactive.

The MIT License applies only to the original source code, documentation, and other original content created for this project. It does not apply to Rockstar Games' intellectual property or copyrighted game assets.

---

# 📄 License

This project is licensed under the **MIT License**. See the **LICENSE** file for more information.

---

# ❤️ Credits

Created by **MbarekTR**

If you use this project in your server or any public project, a credit is appreciated but not required.

Enjoy! 🚀
