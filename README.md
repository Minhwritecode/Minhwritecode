<div align="center">
  
# 👋 Hi, I'm **Michael**  
### Mobile & Web Developer • AI Enthusiast • IoT Builder • IT Lover  

🌌 *“Building things that live in phones, clouds, and tiny sensors.”*

<img src="https://media.giphy.com/media/qgQUggAC3Pfv687qPC/giphy.gif" width="260"/>

</div>

---

## 🧑‍💻 About Me
- 📱 Mobile-Web Dev (React Native / Kotlin / Swift)
- 🤖 AI & Machine Learning (LLMs, Vision, Agents)  
- 📡 IoT Hobbyist (Arduino, ESP32, robotics)  
- 🎨 Love designing futuristic UI (cosmic, cyberpunk)  
- 🐶 Dog lover  
- 📚 Reading books about tech & psychology  
- 💻 Coding on **MacBook** everyday  
- 🔷 Rubik Cube speedsolver & algorithm enthusiast  

---

## 🚀 Tech Stack

### 👨‍💻 Programming
`Java` `Kotlin` `JavaScript` `Python` `C++` `Swift`

### 📱 Mobile
`React Native` `Android Studio` `Kotlin` `Expo` `Flutter`

### 🤖 AI / Data
`TensorFlow` `PyTorch` `OpenCV` `LangChain` `Dify`

### 🌐 Web
`Next.js` `Node.js` `Three.js` `REST API` `React`

### 🔌 IoT
`Arduino` `ESP32` `Sensors` `Servo/Stepper`

---

## 🎯 Featured Projects

| Project | Description | Tech |
|--------|-------------|------|
| 🧠 **AI Virus Detector** | AI app phân tích & cảnh báo sớm bệnh | Python, TensorFlow |
| 🎥 **City Surveillance System** | Dự án phân tích video & AI | JS, Python, OpenCV |
| 📱 **Rubik Cube Solver App** | App giải Rubik bằng camera | React Native, Three.js |
| 🚗 **Smart Arduino Car** | Xe tự hành + Line tracking + AI | Arduino, ESP32 |

---

## 🪄 3D Rubik Animation (Three.js)

> Bạn có thể nhúng trực tiếp 3D model dùng **GitHub Pages + Three.js**  
> Mình cung cấp luôn file nhúng phù hợp cho Profile (link demo sẵn)

### Cách nhúng:
1. Tạo folder `threejs/`
2. Thêm file `index.html` sau (mình viết sẵn):

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<title>3D Rubik</title>
<style> body { margin: 0; background: #000; } canvas { display: block; } </style>
</head>
<body>
<script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js"></script>
<script>
const scene = new THREE.Scene();
scene.background = new THREE.Color("#000000");

const camera = new THREE.PerspectiveCamera(70, window.innerWidth / window.innerHeight, 0.1, 1000);
camera.position.z = 4;

const renderer = new THREE.WebGLRenderer({ antialias: true });
renderer.setSize(window.innerWidth, window.innerHeight);
document.body.appendChild(renderer.domElement);

// Cube
const geometry = new THREE.BoxGeometry();
const edges = new THREE.EdgesGeometry(geometry);
const material = new THREE.LineBasicMaterial({ color: "#0ff" });
const cube = new THREE.LineSegments(edges, material);
scene.add(cube);

function animate() {
    requestAnimationFrame(animate);
    cube.rotation.x += 0.01;
    cube.rotation.y += 0.01;
    renderer.render(scene, camera);
}
animate();
</script>
</body>
</html>
