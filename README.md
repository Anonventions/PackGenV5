# PackGen Pro 🎨📦
**The Ultimate Web-Based Minecraft Resource Pack Generator**

PackGen Pro is a 100% browser-based application designed to take the headache out of making Minecraft `CustomModelData` resource packs. It seamlessly bridges the gap between Blockbench exports and ready-to-play server packs, fully supporting the massive data-driven changes introduced in Minecraft 1.21.4.

## 🌟 Key Features

*   **1.21.4+ Data-Driven Support:** Automatically generates the new `items/` component-based structure required for newer Minecraft versions.
*   **Legacy Pack Converter:** Upload an old 1.14 - 1.20 `.zip` pack, and the engine will instantly scan your old `models/item/` overrides and map them to the new 1.21.4 format!
*   **Multi-Texture Handling:** Attach multiple PNGs to a single model. The engine reads your JSON variables and accurately maps them.
*   **Live Recolor Engine:** Click the Palette icon to hue-shift and saturate your textures inside the browser—create 5 color variants of the same sword without opening Photoshop!
*   **Exact In-Game UI Preview:** A WYSIWYG editor that renders `§a` color codes exactly how they appear in the Minecraft pack selection screen.
*   **True UV 3D Viewer:** Built with Three.js, the 3D viewer parses your JSON UV mapping to accurately project textures onto your model faces.
*   **Project Workspaces:** Save your queue, IDs, and pack settings to a local JSON file and resume your work later.

## 🚀 How to Host / Install

This project is bundled into a single monolithic `index.html` file (with no external CSS/JS files required). 

1. **GitHub Pages:**
   * Fork or clone this repository.
   * Go to your repository settings on GitHub -> **Pages**.
   * Set the source to the `main` branch.
   * Your app is now live!

2. **Local Usage:**
   * Simply download `index.html` and double-click it to open it in Chrome, Firefox, or Edge. Everything runs locally in your browser.

## 🛠️ How to Use (1.21.4+ Workflow)

1. Select **1.21.4+ (Format 46)** from the dropdown.
2. Enter your base item (e.g., `minecraft:stick`).
3. Upload your Blockbench `.json` model and its accompanying `.png` textures.
4. Click **Add to Queue**.
5. When ready, click **Compile .ZIP**. Drop the ZIP into your `resourcepacks` folder!

**Spawn your item in-game:**
```mcfunction
/give @p stick[custom_model_data={floats:[1]}]
```
*(Older versions will use the standard `/give @p stick{CustomModelData:1}` command)*

## 📜 License
This project is open-source and free to use for both personal and commercial Minecraft servers. Have fun modifying it!
