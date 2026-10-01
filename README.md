<br>
<div align="center">
  <h2>
    <a href="https://github.com/MugGod/GodRect/releases/latest">📥 DOWNLOAD LATEST RELEASE</a>
  </h2>
</div>
<br>

<div align="right">
  <h3>🌍 <strong>English</strong> | <a href="README.ru.md">🇷🇺 Русский</a></h3>
</div>

# ⚡ GodRect Extension
<p align="center">
  <img width="32%" alt="Screenshot 2026-10-01 202753" src="https://github.com/user-attachments/assets/be3f4696-cd05-400c-8a9d-5065b77af694" />
  <img width="32%" alt="Screenshot 2026-10-01 202834" src="https://github.com/user-attachments/assets/dac35acd-e5e8-4b25-9cde-c534dfdd51e3" />
  <img width="32%" alt="Screenshot 2026-10-01 202858" src="https://github.com/user-attachments/assets/9a0898bf-c026-4dfc-a9f9-7099c1798652" />
</p>

**GodRect** is a completely free extension for Adobe After Effects designed to simplify the creation of shapes with custom corner parameters, as vanilla AE basically only offers standard roundness. Also, vanilla AE does not have the ability to create grids from shapes located on separate layers (this option exists in vanilla AE only if all shapes are inside a single layer). The extension allows you to quickly place these shapes on a dynamic grid as separate layers. This is important for controlling objects in 3D space, since shapes grouped inside a single standard shape layer cannot have individual 3D parameters.

---

## ✨ Key Features

- **🔲 Advanced Corner Styles:** 
    - Instant creation of shapes with smooth *Beveled* (45° cut) or *Concave* (inward) corners.
    
    - The shape is generated using procedural vector math and Offset filters. 
    
    - Shapes remain basic parametric objects (without being converted to Bezier paths), preserving their full editability.
   
    - Optional addition of a customizable outer Stroke.
    
- **⚡ Smart Grid:**
  - Creation and auto-alignment of a dynamic grid of shape clones. Fully editable on the fly via expressions linking.

  - The system is designed so that the grid can continue to be edited using sliders even without using the extension.

  - Ability to add new shapes to the grid simply by copying the last shape via `Ctrl + D` + `[`. The copied shapes are automatically aligned to the dynamic grid. 

- **🛠️ Edit Mode:** Allows for mass editing of all shapes in a group simultaneously.
  - Automatically finds shapes created via the extension in the composition and selects the entire group of objects.

  - Safe renaming of groups with automatic updating of expressions.

  - Retroactively changing shape parameters or scaling the grid using the **Update Features** button.

  - Safe deletion of the master layer and all its associated clones via **Kill Rects**.


---

## 📦 Installation Instructions

1. Download the `GodRect vX.X.zip` archive from the [Releases](../../releases) section.
2. Extract the contents of the archive into the Adobe CEP extensions system folder:
   - **Windows:** `C:\Program Files (x86)\Common Files\Adobe\CEP\extensions\`
   - **macOS:** `/Library/Application Support/Adobe/CEP/extensions/`

3. **Enable Developer Mode (PlayerDebugMode):**
   Since the extension does not have an official Adobe digital signature, it must be allowed in the system, otherwise After Effects will block it.

   * **For Windows (Automatic):**
     1. Download the `PlayerDebugMode.reg` file from the repository.
     2. Double-click the file.
     3. Read the warning, click Yes, or proceed to the manual option.

   * **For Windows (Manual):**
     1. Press `Win + R`, type `regedit`, and press `Enter`.
     2. Navigate to: `HKEY_CURRENT_USER\Software\Adobe\`
     3. Find the key for the required version of your CSXS package (e.g., `CSXS.11`, `CSXS.12`, etc., depending on the After Effects version). If there is no such key, create it manually.
     4. Inside this key, create a String Value named **`PlayerDebugMode`**.
     5. Change its value to **`1`**.

   * **For macOS:**
     Open the terminal and run the command (replace `11` with the version of your CSXS package if using a different year of After Effects):
     ```bash
     defaults write com.adobe.CSXS.11 PlayerDebugMode 1
     ```

4. Restart After Effects and go to the menu: **Window > Extensions > GodRect**.

<br>
<div align="center">
  <h2>
    <a href="https://github.com/MugGod/GodRect/releases/latest">📥 DOWNLOAD LATEST RELEASE</a>
  </h2>
</div>
<br>
