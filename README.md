# Interactive 3D Jumbo Bag Configurator (Baffle Bag)

An advanced, high-performance web-based 3D configurator built with **Three.js** and **Tailwind CSS**. Designed specifically for visualizing industrial Baffle Jumbo Bags (FIBCs) with real-time interactive parameters, material customization, and high-density particle simulation up to 150,000 particles.

![Baffle Jumbo Bag 3D](https://img.shields.io/badge/Three.js-r128-blue?style=flat-square&logo=three.js)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-CSS-38bdf8?style=flat-square&logo=tailwindcss)
![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Deployed-success?style=flat-square&logo=github)
![License](https://img.shields.io/badge/License-MIT-green.svg?style=flat-square)

---

## 🌟 Key Features

* **Real-time 3D Baffle Bag Modeling:** Custom mathematical deformation simulating physical bag bulging, corner reinforcement, and vertical side seams with orange stitch lines.
* **High-Density Particle Simulation (`InstancedMesh`):** Supports up to **150,000 internal plastic pellets** rendered smoothly at 60 FPS without re-rendering or lag, optimized for real-time slider updates.
* **Custom Baffle Thickness Control:** Adjustable baffle thickness ranging from $1\text{ mm}$ to $8\text{ mm}$ for detailed top-down inspections.
* **Material & Color Customization:** 
  * Adjustable fabric transparency (`Opacity` from 15% to 100%).
  * Dynamic color palettes for the bag body, corner lifting loops, and internal pellets.
* **Top Spout Options:** Toggle between **Open Top (Duffel)** and **Filling Spout**.
* **Responsive Mobile UI:** Fully mobile-friendly interface with a dedicated toggle button to maximize the 3D canvas view on smartphones and tablets.

---

## 🛠️ Tech Stack

* **Rendering Engine:** [Three.js](https://threejs.org/) (WebGL) via CDN with `OrbitControls`
* **Styling:** [Tailwind CSS](https://tailwindcss.com/)
* **Icons:** [FontAwesome 6](https://fontawesome.com/)
* **Architecture:** Object-Oriented JavaScript (ES6+ Classes) packaged in a single self-contained HTML file.

---

## 🎛️ Configurator Parameters

| Parameter | Type | Range / Options | Description |
| :--- | :--- | :--- | :--- |
| **Bulge Pressure** | Slider | $0\% - 120\%$ | Controls the pneumatic inflation/bulging effect of the bag walls. |
| **Fabric Opacity** | Slider | $15\% - 100\%$ | Adjusts transparency to inspect internal baffles and pellets. |
| **Baffle Thickness**| Slider | $1 - 8\text{ mm}$ | Controls the physical thickness of the 4 internal corner baffle panels. |
| **Pellet Count** | Slider | $5,000 - 150,000$ | Adjusts the density of internal plastic resin particles in real time. |
| **Pellet Color** | Palette | Pure White / Black | Changes internal content material color. |
| **Bag Color** | Palette | Raw White, Light Gray, Blue, Orange, Green | Customizes exterior woven polypropylene fabric color. |
| **Loop Color** | Palette | Green, Blue, Orange, Red, White | Customizes corner lifting loop strap colors. |
| **Top Option** | Button | Open Top / Spout | Switches between duffel top and filling spout configurations. |

---

## 🚀 How to Deploy to GitHub Pages

Since this project is contained within a **single `index.html` file**, deploying it to GitHub Pages is extremely straightforward:

1. **Create a GitHub Repository:**
   * Go to [GitHub](https://github.com/) and create a new public repository (e.g., `jumbo-bag-configurator`).

2. **Upload your Code:**
   * Rename your single HTML file to **`index.html`**.
   * Upload `index.html` directly to the repository's main branch (or push via Git):
     ```bash
     git init
     git add index.html
     git commit -m "Initial commit: Interactive 3D Jumbo Bag Configurator"
     git branch -M main
     git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
     git push -u origin main
     ```

3. **Enable GitHub Pages:**
   * Go to your repository on GitHub and click on the **Settings** tab.
   * In the left sidebar, click on **Pages**.
   * Under **Build and deployment > Source**, select **Deploy from a branch**.
   * Under **Branch**, select `main` (or `master`) and keep the folder as `/ (root)`. Click **Save**.

4. **Access your Live App:**
   * After a minute or two, GitHub will provide a live URL (e.g., `https://YOUR_USERNAME.github.io/YOUR_REPOSITORY/`) where your 3D Configurator is hosted!

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
