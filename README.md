[INDEX.HTML](https://github.com/user-attachments/files/25029556/INDEX.HTML)
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>AI Future Tech</title>
  <link rel="stylesheet" href="style.css" />
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
  
</head>
<body>

  <!-- Particle Background -->
  <canvas id="particles"></canvas>

  <!-- Navigation -->
  <header>
    <h1 class="logo">AI<span>Future</span></h1>
    <nav>
      <a href="#services">Services</a>
      <a href="#portfolio">Portfolio</a>
      <a href="#contact">Contact</a>
    </nav>
    
  </header>
  
  <!-- Hero Section -->
  <section class="hero">
    <h2>I build <span id="typing"></span></h2>
    <p>Next-generation AI-powered digital experiences.</p>
    <button>Explore More</button>
  </section>

  <!-- Services -->
  <section id="services" class="section">
    <div class="cards">
      <section id="services" class="section">
  <h3>AI Services</h3>
  <div class="cards">

    <a href="https://deepai.org/chat" target="_blank" class="card service-card">
      <i class="fa-solid fa-robot"></i>
      <h4>AI Chatbots</h4>
      <p>Smart automated conversations</p>
    </a>

    <a href="https://www.ibm.com/think/topics/data-intelligence" target="_blank" class="card service-card">
      <i class="fa-solid fa-chart-line"></i>
      <h4>Data Intelligence</h4>
      <p>Insights powered by AI</p>
    </a>

    <a href="https://aws.amazon.com/ai/?trk=36e94e60-4afc-4f7c-b732-139b1be35182&sc_channel=ps&trk=4bd3427d-426c-4103-b563-4dee1e4af16c&sc_channel=ps&ef_id=:G:s&s_kwcid=AL!4422!10!71605979241308!!!!71606539997996!!487405169!1145692960812696&msclkid=13c5a80529ae1cb3a356c1844d2a35da" target="_blank" class="card service-card">
      <i class="fa-solid fa-brain"></i>
      <h4>Machine Learning</h4>
      <p>Predictive & adaptive systems</p>
    </a>

  </div>
</section>
 

  <!-- Portfolio -->
  <section id="portfolio" class="section dark">
    <h3>Portfolio</h3>
    <div class="cards">
      <div class="card">🤖Neural App UI</div>
      <div class="card">📊Smart Analytics</div>
      <div class="card">🧠Automation Tools</div>
    </div>
  </section>
  
<!-- Contact -->
  <section id="contact" class="section">
    <h3>Contact</h3>
    <form>
      <input type="text" placeholder="Your Name" required />
      <input type="email" placeholder="Your Email" required />
      <textarea placeholder="Your Message"></textarea>
      <button type="submit">Send Message</button>
    </form>
  </section>


  <script src="script.js"></script>
</body>
</html>

[STYLE.CSS](https://github.com/user-attachments/files/25029560/STYLE.CSS)* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Montserrat', sans-serif;
}

body {
  background: radial-gradient(circle at top, #0a0f1f, #05070d);
  color: white;
  overflow-x: hidden;
}

/* Particle Canvas */
#particles {
  position: fixed;
  width: 100%;
  height: 100%;
  z-index: -1;
}

/* Header */
header {
  display: flex;
  justify-content: space-between;
  padding: 20px 8%;
  position: fixed;
  width: 100%;
  background: rgba(0,0,0,0.4);
  backdrop-filter: blur(10px);
}

.logo span {
  color: cyan;
}

nav a {
  margin-left: 20px;
  color: #ccc;
  text-decoration: none;
  transition: 0.3s;
}

nav a:hover {
  color: cyan;
}

/* Hero */
.hero {
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding-left: 10%;
}

.hero h2 {
  font-size: 3rem;
}

.hero span {
  color: #00ffff;
  border-right: 2px solid cyan;
}

.hero button {
  margin-top: 20px;
  padding: 12px 25px;
  border: none;
  background: linear-gradient(90deg, cyan, magenta);
  color: black;
  font-weight: bold;
  cursor: pointer;
  border-radius: 30px;
}

/* Sections */
.section {
  padding: 100px 8%;
  text-align: center;
}

.dark {
  background: #0c1222;
}

.cards {
  display: flex;
  justify-content: center;
  gap: 30px;
  margin-top: 40px;
  flex-wrap: wrap;
}

.card {
  padding: 40px;
  width: 250px;
  background: rgba(255,255,255,0.05);
  border: 1px solid rgba(0,255,255,0.2);
  border-radius: 15px;
  transition: 0.3s;
}

.card:hover {
  transform: translateY(-10px);
  box-shadow: 0 0 20px cyan;
}

/* Contact */
form {
  display: flex;
  flex-direction: column;
  max-width: 400px;
  margin: auto;
  gap: 25px;
}

input, textarea {
  padding: 10px;
  border-radius: 8px;
  border: none;
}

button {
  cursor: pointer;
}

/* Responsive */
@media(max-width: 768px) {
  .cards {
    flex-direction: column;
    align-items: center;
  }
}

/* Demo Section */
.demo-container {
  margin: 40px auto;
  width: 100%;
  max-width: 1100px;
  height: 600px;
  border-radius: 15px;
  overflow: hidden;
  border: 1px solid rgba(0,255,255,0.3);
  box-shadow: 0 0 25px rgba(0,255,255,0.2);
}

.demo-container iframe {
  width: 100%;
  height: 100%;
  border: none;
}

.demo-btn {
  display: inline-block;
  margin-top: 25px;
  padding: 12px 30px;
  border-radius: 30px;
  background: linear-gradient(90deg, cyan, magenta);
  color: black;
  font-weight: bold;
  text-decoration: none;
  transition: 0.3s;
}

.service-card {
  text-decoration: none;
  color: white;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 15px;
}

.service-card i {
  font-size: 40px;
  color: cyan;
  transition: 0.3s;
}

.service-card h4 {
  font-size: 20px;
}

.service-card p {
  font-size: 14px;
  color: #aaa;
}

/* Hover Animation */
.service-card:hover i {
  transform: scale(1.2);
  color: magenta;
}


[SCRIPT.JS](https://github.com/user-attachments/files/25029564/SCRIPT.JS)
// Typing Effect
const words = ["AI Websites", "Smart Solutions", "Future Experiences"];
let i = 0, j = 0, currentWord = "", isDeleting = false;

function type() {
  currentWord = words[i];
  document.getElementById("typing").textContent =
    currentWord.substring(0, j);

  if (!isDeleting && j < currentWord.length) {
    j++;
    setTimeout(type, 100);
  } else if (isDeleting && j > 0) {
    j--;
    setTimeout(type, 50);
  } else {
    isDeleting = !isDeleting;
    if (!isDeleting) i = (i + 1) % words.length;
    setTimeout(type, 800);
  }
}
type();

// Particle Background
const canvas = document.getElementById("particles");
const ctx = canvas.getContext("2d");
canvas.width = window.innerWidth;
canvas.height = window.innerHeight;

let particles = [];

for (let i = 0; i < 80; i++) {
  particles.push({
    x: Math.random() * canvas.width,
    y: Math.random() * canvas.height,
    radius: Math.random() * 2,
    dx: Math.random() - 0.5,
    dy: Math.random() - 0.5
  });
}

function animateParticles() {
  ctx.clearRect(0, 0, canvas.width, canvas.height);
  ctx.fillStyle = "cyan";

  particles.forEach(p => {
    p.x += p.dx;
    p.y += p.dy;

    if (p.x < 0 || p.x > canvas.width) p.dx *= -1;
    if (p.y < 0 || p.y > canvas.height) p.dy *= -1;

    ctx.beginPath();
    ctx.arc(p.x, p.y, p.radius, 0, Math.PI * 2);
    ctx.fill();
  });

  requestAnimationFrame(animateParticles);
}
animateParticles();



