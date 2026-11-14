# 🌃 Cyber CSS City — Isometric Cyberpunk Traffic Simulator

<p align="center">
  <strong>A futuristic isometric cyberpunk city built entirely with HTML5 and CSS3.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-Structure-orange?style=for-the-badge&logo=html5" alt="HTML5">
  <img src="https://img.shields.io/badge/CSS3-3D%20Transforms-blue?style=for-the-badge&logo=css3" alt="CSS3">
  <img src="https://img.shields.io/badge/JavaScript-Not%20Required-lightgrey?style=for-the-badge" alt="No JavaScript">
  <img src="https://img.shields.io/badge/Responsive-Design-success?style=for-the-badge" alt="Responsive design">
</p>

---

## 🚀 Project Overview

**Cyber CSS City** is an experimental front-end project that explores the creation of an isometric cyberpunk environment using only HTML and CSS.

The project transforms ordinary HTML elements into a layered futuristic city featuring 3D-style buildings, illuminated windows, neon streets, animated vehicles, glowing streetlights, and an atmospheric night environment.

It demonstrates how CSS transforms, perspective, preserved 3D rendering contexts, keyframe animations, gradients, shadows, and custom properties can work together to create an animated visual experience without JavaScript or external graphics libraries.

## 🌐 Live Demo

**GitHub Repository:**  
https://github.com/Regalson001/cyber-css-city

**Live Website:**  
https://regalson001.github.io/cyber-css-city/

*The live demo becomes available after successfully enabling GitHub Pages.*

## ✨ Key Features

### 1. Isometric 3D City Environment
- Isometric city presentation using CSS transforms.
- Perspective-based 3D stage.
- Layered city ground and building structures.
- Multiple building faces created using HTML elements.
- CSS grid alignment for the urban environment.

### 2. Cyberpunk Architecture
- Five futuristic building structures.
- Front, side, and top building faces.
- Neon building borders.
- Glowing architectural details.
- Animated window illumination.
- Custom building signs.

### 3. Animated Traffic System
- Multiple vehicles moving along horizontal and vertical roads.
- Continuous looping CSS animations.
- Different vehicle colours.
- Independent animation durations and delays.
- Neon vehicle lighting effects.

### 4. Neon Lighting Environment
- Glowing streetlights.
- Animated lighting effects.
- Cyan, purple, pink, yellow, and green accents.
- Layered shadows and radial gradients.
- Animated background stars.

### 5. Engineering Dashboard
- Architecture information cards.
- Traffic system information.
- Lighting system overview.
- CSS 3D technology summary.

### 6. Responsive Interface
- Desktop, tablet, and mobile layouts.
- CSS Grid and Flexbox.
- Responsive typography using `clamp()`.
- Media queries for smaller screens.
- Reduced-motion accessibility support.

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| HTML5 | Semantic page structure |
| CSS3 | Complete visual design |
| CSS 3D Transforms | Isometric environment |
| CSS Perspective | 3D depth presentation |
| CSS Grid | City layout and dashboard |
| CSS Flexbox | Interface alignment |
| CSS Variables | Reusable design tokens |
| CSS Keyframes | Traffic and lighting animations |
| CSS Gradients | Neon atmosphere and surfaces |
| CSS Media Queries | Responsive design |

**No JavaScript, frameworks, external libraries, or build tools are required.**

## 🧠 Advanced CSS Techniques Demonstrated

### 1. CSS 3D Transformations

The city stage uses 3D transforms to create an isometric viewing angle.

```css
.city-ground {
  transform-style: preserve-3d;
  transform: rotateX(57deg) rotateZ(-45deg);
}
```

The `rotateX()` and `rotateZ()` functions establish the isometric perspective.

### 2. Preserving 3D Space

Nested elements use:

```css
transform-style: preserve-3d;
```

This allows transformed child elements to maintain their 3D positioning within the parent rendering context.

### 3. CSS Perspective

The scene uses:

```css
.city-stage {
  perspective: 1100px;
  perspective-origin: 50% 45%;
}
```

Perspective controls how depth is visually presented.

### 4. Layered Building Geometry

Buildings are constructed from separate HTML elements representing:

- Front face.
- Side face.
- Top face.

These surfaces use `translateZ()`, `rotateX()`, and `rotateY()` to create a 3D-style structure.

### 5. Multi-Stage CSS Animations

Vehicles move along the roads using independent keyframes.

Example:

```css
@keyframes drive-right {
  from {
    left: -45px;
  }

  to {
    left: calc(100% + 45px);
  }
}
```

Different animation durations and delays create varied traffic movement.

### 6. Neon Lighting and Glow Effects

The project uses multiple layers of `box-shadow`, `text-shadow`, gradients, and opacity to create a futuristic lighting environment.

### 7. CSS Custom Properties

Reusable design tokens are defined in `:root`:

```css
:root {
  --cyan: #35e9ff;
  --pink: #ff3eb5;
  --purple: #9b5cff;
  --yellow: #ffe66d;
  --green: #45ffb0;
}
```

This makes it easier to adjust the city's visual theme.

### 8. Responsive Design

Media queries adjust the scene's scale, dashboard layout, and typography for different screen sizes.

## 📂 Project Structure

```text
cyber-css-city/
│
├── index.html
│   └── Main HTML structure
│
├── styles.css
│   └── 3D city, styling, and animations
│
├── README.md
│   └── Project documentation
│
├── LICENSE
│   └── MIT License
│
└── .gitignore
    └── Files excluded from Git
```

## ⚙️ Getting Started

### Prerequisites

- A modern web browser.
- Visual Studio Code or another code editor.
- Git installed on your computer.
- A GitHub account for publishing the project.

### 1. Clone the Repository

```bash
git clone https://github.com/Regalson001/cyber-css-city.git
```

### 2. Navigate to the Project Folder

```bash
cd cyber-css-city
```

### 3. Open in Visual Studio Code

```bash
code .
```

### 4. Run the Project

Open `index.html` in your browser.

Alternatively, use the Live Server extension in Visual Studio Code.

The city and traffic animations start automatically when the page loads.

## 🎯 Learning Objectives

This project provides practical experience with:

- Creating isometric visual environments.
- Understanding CSS 3D coordinate transformations.
- Using `perspective` and `transform-style`.
- Building 3D-style structures from HTML elements.
- Positioning nested elements in transformed coordinate spaces.
- Creating synchronized and independent CSS animations.
- Designing neon lighting effects.
- Using CSS custom properties for consistent styling.
- Building responsive interfaces.
- Applying reduced-motion accessibility preferences.

## ⚠️ Project Scope and Limitations

This is a visual CSS simulation, not a real-time traffic or urban-planning engine.

- Vehicles follow predefined CSS animation paths.
- There is no collision detection or traffic intelligence.
- Buildings are CSS-rendered visual structures, not 3D models.
- No real city map, geographical data, or navigation system is connected.
- The dashboard displays illustrative project information rather than live sensor readings.
- No JavaScript or backend service is used.

## 🔮 Future Improvements

Possible future development ideas:

- Add more buildings and city districts.
- Create animated pedestrian crossings.
- Introduce traffic signals and intersection lights.
- Add multiple traffic lanes.
- Create animated trains or flying vehicles.
- Add day and night visual themes.
- Build a CSS-controlled zoom and camera interface.
- Introduce more complex building geometry.
- Explore interactive city controls in a future JavaScript version.

## 📸 Project Preview

Add a screenshot of your completed project to the repository.

Recommended structure:

```text
cyber-css-city/
│
└── assets/
    └── cyber-city-preview.png
```

Then add the following to this README:

```markdown
![Cyber CSS City Preview](./assets/cyber-city-preview.png)
```

A high-quality screenshot or GIF will help visitors understand the project immediately.

## 🌍 Deployment with GitHub Pages

This project can be deployed for free using GitHub Pages.

1. Open the repository on GitHub.
2. Navigate to **Settings**.
3. Select **Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Select branch `main`.
6. Select folder `/(root)`.
7. Click **Save**.

After GitHub finishes deploying, your portfolio project will be available at:

https://regalson001.github.io/cyber-css-city/

## 👨‍💻 Author

**Stephen Oyugi**

Front-End Developer | AI Automation Practitioner | Machine Learning Practitioner

📍 Nairobi, Kenya

- **GitHub:** https://github.com/Regalson001
- **LinkedIn:** https://linkedin.com/in/stephenoyugi001
- **Email:** stephennyarangi03@gmail.com

## 📄 License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

<p align="center">
  <strong>Designed and developed by Stephen Oyugi.</strong>
</p>

<p align="center">
  Building interfaces. Exploring dimensions. Engineering with CSS.
</p>
