# GSAP Animations Demo Project 🎨

Welcome to the GSAP Animations Demo Project! This project demonstrates various concepts and features of the GreenSock Animation Platform (GSAP). 

## 🧠 Concepts Covered:

- ✨ How to install GSAP
- ⏱️ How to create timelines in GSAP
- 🏎️ Modifying animation speed in GSAP
- 🔄 Reversing GSAP animations

## 🚀 Getting Started

To get started with this project, you need to include the GSAP library in your project. You can do this by adding the following CDN link to your HTML file:

```html
<script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.9.1/gsap.min.js"></script>
```

## 📂 Project Structure

```
/gsap-animations-demo
|-- index.html
|-- styles.css
|-- script.js
```

### 🔧 Installation

1. Clone this repository:
   ```sh
   git clone https://github.com/manvendra2000/gsap-animations-demo.git
   ```

2. Navigate to the project directory:
   ```sh
   cd gsap-animations-demo
   ```

3. Open `index.html` in your browser to see the demo.

### 📝 Usage

In your `script.js` file, you can start creating animations with GSAP:

```javascript
// Basic GSAP Animation
gsap.to(".box", {duration: 2, x: 100});

// Creating a Timeline
const tl = gsap.timeline();
tl.to(".box", {duration: 1, x: 100})
  .to(".box", {duration: 1, y: 100})
  .to(".box", {duration: 1, x: 0})
  .to(".box", {duration: 1, y: 0});

// Modifying Animation Speed
gsap.to(".box", {duration: 0.5, rotation: 360});

// Reversing Animations
const animation = gsap.to(".box", {duration: 2, x: 100});
document.getElementById("reverseBtn").addEventListener("click", () => {
  animation.reverse();
});
```

### 📦 Dependencies

This project uses GSAP, included via CDN. No other dependencies are required.

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to clone, explore, and modify the project to learn more about GSAP animations! 🌟
