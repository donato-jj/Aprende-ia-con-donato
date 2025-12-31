

/* Estilo actualizado: Futurista, profesional, con estrellas y "AI vibes" */
/* Variables y tipografía */
:root{
  --bg-0: #040617;
  --bg-1: #071028;
  --glass: rgba(255,255,255,0.06);
  --glass-2: rgba(255,255,255,0.04);
  --accent: #00e5ff;
  --accent-2: #7c3cff;
  --neon: 0, 229, 255; /* RGB para glow */
  --card-radius: 14px;
  --glass-border: linear-gradient(135deg, rgba(255,255,255,0.06), rgba(255,255,255,0.02));
}

@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&display=swap');

*{box-sizing:border-box}
html,body{height:100%}

body {
  margin: 0;
  font-family: "Inter", Arial, sans-serif;
  background: radial-gradient(1200px 600px at 10% 10%, rgba(124,60,255,0.09), transparent),
              radial-gradient(900px 500px at 90% 90%, rgba(0,229,255,0.05), transparent),
              linear-gradient(180deg, var(--bg-0), var(--bg-1) 60%);
  color: #eaf6ff;
  -webkit-font-smoothing:antialiased;
  -moz-osx-font-smoothing:grayscale;
  position:relative;
  overflow-x:hidden;
  min-height:100vh;
}

/* Estrella / campo estelar animado (pseudo-elemento) */
body::before{
  content:"";
  position:fixed;
  inset:0;
  z-index:0;
  background-image:
    radial-gradient(1px 1px at 5% 10%, rgba(255,255,255,0.9), transparent 40%),
    radial-gradient(1px 1px at 15% 50%, rgba(255,255,255,0.85), transparent 40%),
    radial-gradient(1px 1px at 30% 20%, rgba(255,255,255,0.75), transparent 40%),
    radial-gradient(1px 1px at 60% 80%, rgba(255,255,255,0.65), transparent 40%),
    radial-gradient(1px 1px at 85% 25%, rgba(255,255,255,0.6), transparent 40%),
    radial-gradient(2px 2px at 45% 40%, rgba(255,255,255,0.35), transparent 40%),
    radial-gradient(0.8px 0.8px at 75% 70%, rgba(255,255,255,0.45), transparent 40%);
  background-size: 1200px 800px, 1000px 700px, 800px 600px, 700px 500px, 600px 400px, 1400px 1000px, 900px 600px;
  opacity:0.45;
  animation: starfield 60s linear infinite;
  pointer-events:none;
  filter: blur(0.6px);
}

@keyframes starfield{
  from{transform:translate3d(0,0,0)}
  to{transform:translate3d(-1200px,-800px,0)}
}

/* Contenedor principal para situar encima del fondo */
.container{
  position:relative;
  z-index:1;
  max-width:1100px;
  margin:0 auto;
  padding:40px 20px 120px;
}

/* Hero mejorado */
.hero {
  text-align: left;
  padding: clamp(36px, 6vw, 88px);
  border-radius: 18px;
  background: linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
  box-shadow: 0 10px 40px rgba(2,6,23,0.6), inset 0 1px 0 rgba(255,255,255,0.02);
  display:flex;
  gap:28px;
  align-items:center;
  backdrop-filter: blur(8px);
  -webkit-backdrop-filter: blur(8px);
  border: 1px solid rgba(255,255,255,0.03);
  position:relative;
  overflow:visible;
}

.hero .content{
  flex:1;
  padding-right:20px;
}

.hero h1{
  font-size:clamp(1.8rem, 4vw, 3.6rem);
  margin:0 0 8px 0;
  line-height:1.02;
  letter-spacing:-0.02em;
  color: linear-gradient(90deg, #fff, #e6f9ff);
  text-shadow: 0 6px 28px rgba(var(--neon),0.06), 0 2px 4px rgba(0,0,0,0.6);
  font-weight:800;
}

.hero p{
  margin:0 0 18px;
  color:rgba(234,246,255,0.9);
  font-size:1.05rem;
}

/* Botones neon */
.btn {
  display: inline-flex;
  align-items:center;
  gap:10px;
  padding: 12px 26px;
  background: linear-gradient(90deg, rgba(0,229,255,0.12), rgba(124,60,255,0.12));
  color: var(--accent);
  text-decoration: none;
  border-radius: 999px;
  border: 1px solid rgba(255,255,255,0.06);
  box-shadow: 0 6px 30px rgba(0,0,0,0.6), 0 0 18px rgba(var(--neon),0.06);
  transition: transform .18s ease, box-shadow .18s ease;
  font-weight:600;
}
.btn .dot{
  width:10px; height:10px; border-radius:50%;
  background:linear-gradient(180deg,var(--accent),var(--accent-2));
  box-shadow:0 0 12px rgba(var(--neon),0.8);
}

/* Hover effect */
.btn:hover, .btn:focus{
  transform: translateY(-4px);
  box-shadow: 0 18px 40px rgba(var(--neon),0.16), 0 0 36px rgba(var(--neon),0.12);
  color: #001a1f;
  background: linear-gradient(90deg, var(--accent), var(--accent-2));
}

/* Visual AI area (SVG or canvas) */
.ai-visual {
  width:360px;
  height:220px;
  border-radius: 12px;
  background: linear-gradient(180deg, rgba(0,0,0,0.18), rgba(255,255,255,0.02));
  border: 1px solid rgba(255,255,255,0.04);
  display:flex;
  align-items:center;
  justify-content:center;
  position:relative;
  overflow:hidden;
  box-shadow: 0 10px 36px rgba(12,22,40,0.6), 0 0 40px rgba(var(--neon),0.06);
  flex-shrink:0;
}

/* Neon network (SVG will sit inside and animate via CSS) */
.ai-visual svg{ width:100%; height:100%; display:block; }

/* Section generic */
section {
  padding: 60px 0;
  text-align: center;
  position:relative;
  z-index:1;
}

/* Grid modern */
.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
  gap: 20px;
  margin-top:18px;
}

/* Card with glassmorphism + gradient border */
.grid div {
  background: linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
  padding: 22px;
  border-radius: var(--card-radius);
  border: 1px solid rgba(255,255,255,0.03);
  box-shadow: 0 8px 28px rgba(2,8,28,0.6);
  backdrop-filter: blur(6px);
  -webkit-backdrop-filter: blur(6px);
  transition: transform .22s ease, box-shadow .22s ease;
  position:relative;
  overflow:hidden;
}

/* Animated gradient accent stripe */
.grid div::before{
  content:"";
  position:absolute;
  inset:auto 0 0 0;
  height:4px;
  background: linear-gradient(90deg, transparent, rgba(124,60,255,0.9), rgba(0,229,255,0.9), transparent);
  transform:translateY(100%);
  transition:transform .28s cubic-bezier(.2,.9,.2,1);
}

/* Hover lifts and reveals accent */
.grid div:hover{
  transform: translateY(-8px);
  box-shadow: 0 18px 60px rgba(12,22,40,0.7);
}
.grid div:hover::before{ transform:translateY(0%) }

/* Contact form */
.contact {
  display:flex;
  flex-direction:column;
  align-items:center;
  gap:8px;
}
.contact input, .contact textarea {
  width: 95%;
  max-width:720px;
  padding: 12px 14px;
  margin: 8px 0;
  border-radius: 10px;
  border: 1px solid rgba(255,255,255,0.04);
  background: rgba(255,255,255,0.02);
  color: #eaf6ff;
  outline:none;
  resize:vertical;
  box-shadow: inset 0 1px 0 rgba(255,255,255,0.02);
}
.contact input:focus, .contact textarea:focus{
  border-color: rgba(var(--neon),0.9);
  box-shadow: 0 6px 30px rgba(var(--neon),0.06);
}

/* Footer */
footer {
  background: linear-gradient(180deg, rgba(0,0,0,0.6), rgba(4,6,10,0.8));
  padding: 28px 20px;
  text-align: center;
  color: rgba(234,246,255,0.7);
  border-top: 1px solid rgba(255,255,255,0.02);
}

/* Utility */
.center { text-align:center }
.kicker { color: rgba(234,246,255,0.65); font-weight:600; margin-bottom:10px; text-transform:uppercase; letter-spacing:0.14em; font-size:0.75rem }

/* Small screens adjustments */
@media (max-width:880px){
  .hero{ flex-direction:column; padding:28px }
  .ai-visual{ width:100%; height:200px; order:2 }
  .hero .content{ order:1; padding-right:0 }
}

/* Respect reduced motion */
@media (prefers-reduced-motion:reduce){
  * { animation-duration: 0.001ms !important; animation-iteration-count: 1 !important; transition-duration: 0.001ms !important; scroll-behavior: auto !important; }
}

