# Casa-SM Interactive Electrical Design & Simulation Software

An interactive, web-based CAD tool specifically designed for visualizing, mapping, and testing the electrical layout of the **Casa-SM** residential project. Built purely with modern web technologies, it allows users to overlay dynamic electrical circuits directly onto architectural blueprints, bundle wall switches into modular vertical boxes, and test configurations using a live grid simulation mode.

## 🚀 Live Demo

You can run and test this application directly from your browser without installing anything:
👉 **[LAUNCH LIVE APP](https://YOUR_GITHUB_USERNAME.github.io/YOUR_REPOSITORY_NAME/)** *(Replace with your actual GitHub Pages link once enabled)*

---

## ✨ Features

- **Dynamic Blueprint Mapping:** Precision point-and-click placement of components aligned to the underlying scale of architectural plans (`IE_01`).
- **Diverse Luminarie Subtypes:** Fully supports 3 distinct lighting modules with custom spatial representations:
  - 💡 **Standard Lights:** Circular residential general-purpose overhead outlets.
  - 🔳 **Floodlights/Reflectors:** Squared exterior projectors featuring targeted high-intensity lighting beams.
  - ➖/🪟 **LED Light Strips:** Directional linear modules configurable in either **Horizontal** or **Vertical** orientations.
- **Smart Modular Switch Boxes (Cambre/Sica Style):** Clean up blueprint clutter by multi-selecting (`CTRL` + Click) overlapping wall switches and grouping them into sleek, compact vertical wall faceplates.
- **Live Energy Simulation Mode:** Activate the grid to toggle power distribution. Grouped switch plates display independent live feedback—individual keys dynamically switch to green when their connected sub-circuit is powered.
- **Dynamic Deconstruct Feature:** Mistakenly grouped a box? A simple **Right-Click** disassembles any modular faceplate, resetting switches back to their exact original layout positions.
- **JSON Project Version Control:** Full **Export** and **Import** functionality allows you to save independent iterations (e.g., `circuit_v1.json`, `circuit_v2_unified.json`) locally and pick up right where you left off.

---

## 🛠️ Technology Stack

- **Frontend:** HTML5, CSS3 (Modern Flexbox grid, CSS Variable architecture, Keyframe Animations).
- **Interactions:** Native Vanilla JavaScript DOM manipulation, multi-pointer Drag-and-Drop system, custom Context Menu event listeners.
- **Data Persistence:** Client-side JSON file encoding & parsing utilizing `FileReader` streams.

---

## 📂 Installation & Local Usage

Since the architecture is built completely on client-side environments, there are no server-side compilers or node packages required.

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/YOUR_GITHUB_USERNAME/YOUR_REPOSITORY_NAME.git](https://github.com/YOUR_GITHUB_USERNAME/YOUR_REPOSITORY_NAME.git)