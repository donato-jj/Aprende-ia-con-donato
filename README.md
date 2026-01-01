<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Aprendizaje de IA | Futuro Tecnológico</title>

<style>
/* ================= RESET ================= */
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Segoe UI', Tahoma, sans-serif;
}

/* ================= BODY ================= */
body{
    background: radial-gradient(circle at top, #0b0220, #02000a 70%);
    color:#eaeaff;
    overflow-x:hidden;
}

/* ================= HEADER ================= */
header{
    padding:60px 20px;
    text-align:center;
}

header h1{
    font-size:3rem;
    color:#7df9ff;
    text-shadow:0 0 20px #00f0ff;
    animation: glow 3s infinite alternate;
}

header p{
    max-width:800px;
    margin:20px auto 0;
    color:#cfcfff;
}

/* ================= SECTIONS ================= */
section{
    padding:80px 10%;
    position:relative;
}

section h2{
    font-size:2.2rem;
    color:#b98cff;
    margin-bottom:20px;
}

section p, section li{
    line-height:1.7;
    color:#ddddff;
}

ul{
    margin-left:20px;
}

/* ================= FUTURISTIC DIVIDER ================= */
.divider{
    height:2px;
    background:linear-gradient(90deg, transparent, #7df9ff, transparent);
    margin:60px 0;
}

/* ================= ALIENS & ROBOTS ================= */
.alien, .robot{
    position:absolute;
    width:60px;
    height:60px;
    border-radius:50%;
    filter:drop-shadow(0 0 10px #00f0ff);
}

.alien{
    background:radial-gradient(circle, #00ffcc, #006666);
    animation: floatAlien 12s linear infinite;
}

.robot{
    background:linear-gradient(135deg, #999, #444);
    border-radius:10px;
    animation: walkRobot 10s linear infinite;
}

.alien::after{
    content:'';
    position:absolute;
    top:15px;
    left:15px;
    width:8px;
    height:8px;
    background:#000;
    border-radius:50%;
    box-shadow:20px 0 #000;
}

.robot::after{
    content:'';
    position:absolute;
    bottom:-10px;
    left:10px;
    width:40px;
    height:10px;
    background:#222;
}

/* ================= CONTACT ================= */
.contact{
    text-align:center;
    padding:80px 20px;
}

.buttons{
    display:flex;
    justify-content:center;
    gap:25px;
    flex-wrap:wrap;
}

.btn{
    padding:15px 30px;
    border-radius:40px;
    text-decoration:none;
    color:#fff;
    font-weight:bold;
    background:linear-gradient(135deg, #6a00ff, #00f0ff);
    box-shadow:0 0 20px rgba(0,240,255,.6);
    transition:all .4s ease;
}

.btn:hover{
    transform:scale(1.1);
    box-shadow:0 0 35px #7df9ff;
}

/* ================= FOOTER ================= */
footer{
    text-align:center;
    padding:30px;
    color:#888;
    font-size:.9rem;
}

/* ================= ANIMATIONS ================= */
@keyframes glow{
    from{ text-shadow:0 0 10px #00f0ff; }
    to{ text-shadow:0 0 30px #7df9ff; }
}

@keyframes floatAlien{
    0%{ left:-10%; top:20%; }
    100%{ left:110%; top:40%; }
}

@keyframes walkRobot{
    0%{ right:-10%; bottom:10%; }
    100%{ right:110%; bottom:15%; }
}

/* ================= CHATBOX ================= */
#chat-container{
    position:fixed;
    bottom:20px;
    right:20px;
    width:320px;
    max-width:90%;
    background:rgba(15,0,40,0.95);
    border:2px solid #7df9ff;
    border-radius:15px;
    box-shadow:0 0 25px #00f0ff;
    display:flex;
    flex-direction:column;
    font-size:0.95rem;
    z-index:9999;
}

#chat-header{
    background:linear-gradient(135deg, #6a00ff, #00f0ff);
    padding:12px;
    border-top-left-radius:12px;
    border-top-right-radius:12px;
    color:#fff;
    font-weight:bold;
    cursor:pointer;
    text-align:center;
}

#chat-messages{
    flex:1;
    padding:10px;
    overflow-y:auto;
    max-height:300px;
    color:#e0e0ff;
}

.message{
    margin-bottom:12px;
    padding:8px 12px;
    border-radius:12px;
    max-width:80%;
    word-wrap:break-word;
}

.message.user{
    background:#1a1a2e;
    align-self:flex-end;
    color:#7df9ff;
}

.message.bot{
    background:#33334d;
    align-self:flex-start;
    color:#fffcaa;
}

#chat-input-container{
    display:flex;
    border-top:1px solid #444;
}

#chat-input{
    flex:1;
    padding:10px;
    border:none;
    border-radius:0 0 0 12px;
    background:#0b0220;
    color:#fff;
}

#chat-input:focus{
    outline:none;
}

#chat-send{
    padding:0 20px;
    border:none;
    background:#7df9ff;
    color:#000;
    font-weight:bold;
    cursor:pointer;
    border-radius:0 0 12px 0;
    transition:0.3s;
}

#chat-send:hover{
    background:#00f0ff;
}

/* Scrollbar */
#chat-messages::-webkit-scrollbar{
    width:6px;
}
#chat-messages::-webkit-scrollbar-thumb{
    background:#7df9ff;
    border-radius:3px;
}
</style>
</head>

<body>

<header>
    <h1>Aprendizaje del Futuro</h1>
    <p>Exploramos la Inteligencia Artificial y la Programación como pilares de la tecnología avanzada del mañana.</p>
</header>

<div class="alien"></div>
<div class="robot"></div>

<section>
    <h2>🧠 Aprendizaje de Inteligencia Artificial</h2>
    <p>
        El aprendizaje de Inteligencia Artificial es el proceso mediante el cual las máquinas adquieren la capacidad
        de analizar datos, aprender patrones y tomar decisiones inteligentes sin intervención humana constante.
    </p>
    <ul>
        <li>Aprendizaje supervisado</li>
        <li>Aprendizaje no supervisado</li>
        <li>Aprendizaje profundo (Deep Learning)</li>
        <li>Redes neuronales artificiales</li>
    </ul>
    <p>
        La IA se aplica en medicina, robótica, finanzas, automatización, análisis de datos y exploración espacial,
        permitiendo un futuro más eficiente, inteligente y conectado.
    </p>
</section>

<div class="divider"></div>

<section>
    <h2>💻 Aprendizaje de Programación</h2>
    <p>
        La programación es la base del mundo digital. Aprender a programar desarrolla la lógica, el pensamiento crítico
        y la capacidad de crear soluciones tecnológicas reales.
    </p>
    <ul>
        <li>Fundamentos de programación</li>
        <li>Introducción a Python</li>
        <li>Lógica y estructuras de control</li>
        <li>Automatización y análisis de datos</li>
    </ul>
    <p>
        Python es uno de los lenguajes más usados en Inteligencia Artificial por su simplicidad, potencia y versatilidad,
        siendo clave en el desarrollo de sistemas inteligentes.
    </p>
</section>

<div class="divider"></div>

<section class="contact">
    <h2>📡 Contacto Futurista</h2>
    <div class="buttons">
        <a class="btn" href="https://wa.me/2235319300" target="_blank">WhatsApp</a>
        <a class="btn" href="https://www.instagram.com/donato%20acosta%2012/" target="_blank">Instagram</a>
        <a class="btn" href="mailto:donatoconturla100@gmail.com">Gmail</a>
    </div>
</section>

<footer>
    © Futuro IA · Tecnología Avanzada · Diseño Futurista
</footer>

<!-- ================= CHATBOX ================= -->
<div id="chat-container">
    <div id="chat-header">🤖 Asistente IA</div>
    <div id="chat-messages"></div>
    <div id="chat-input-container">
        <input type="text" id="chat-input" placeholder="Escribe tu pregunta..." />
        <button id="chat-send">Enviar</button>
    </div>
</div>

<script>
const chatContainer = document.getElementById('chat-container');
const chatHeader = document.getElementById('chat-header');
const chatMessages = document.getElementById('chat-messages');
const chatInput = document.getElementById('chat-input');
const chatSend = document.getElementById('chat-send');

let chatOpen = true;
chatHeader.addEventListener('click', () => {
    chatOpen = !chatOpen;
    chatMessages.style.display = chatOpen ? 'block' : 'none';
    document.getElementById('chat-input-container').style.display = chatOpen ? 'flex' : 'none';
});

function addMessage(text, sender){
    const msg = document.createElement('div');
    msg.classList.add('message', sender);
    msg.textContent = text;
    chatMessages.appendChild(msg);
    chatMessages.scrollTop = chatMessages.scrollHeight;
}

// Función básica de IA usando reglas simples
function aiResponse(userText){
    const text = userText.toLowerCase();

    if(/(aprendizaje supervisado|supervisado)/.test(text)){
        return "El aprendizaje supervisado consiste en entrenar modelos usando datos etiquetados para que puedan predecir resultados futuros.";
    }
    if(/(aprendizaje no supervisado|no supervisado)/.test(text)){
        return "El aprendizaje no supervisado busca patrones en datos sin etiquetas, ideal para agrupamiento o reducción de dimensiones.";
    }
    if(/deep learning|aprendizaje profundo/.test(text)){
        return "El Deep Learning utiliza redes neuronales profundas para resolver problemas complejos como visión por computadora y procesamiento de lenguaje natural.";
    }
    if(/python/.test(text)){
        return "Python es un lenguaje versátil y muy usado en Inteligencia Artificial. Puedes usarlo para automatización, análisis de datos y desarrollo de modelos de IA.";
    }
    if(/programación|lógica|estructura/.test(text)){
        return "Aprender programación fortalece la lógica y la resolución de problemas. Python es excelente para empezar y luego avanzar a proyectos de IA.";
    }
    if(/contacto|whatsapp|instagram|gmail/.test(text)){
        return "Puedes contactarnos vía WhatsApp, Instagram o Gmail usando los botones en la sección de contacto.";
    }
    if(/hola|buenos días|buenas tardes|hey/.test(text)){
        return "¡Hola! Soy tu asistente IA, listo para responder tus consultas sobre Inteligencia Artificial y programación.";
    }
    return "Lo siento, no entendí tu pregunta. Puedes preguntarme sobre IA, Python, Deep Learning o cómo contactarnos.";
}

function sendMessage(){
    const userText = chatInput.value.trim();
    if(userText === "") return;

    addMessage(userText, 'user');
    chatInput.value = '';

    setTimeout(() => {
        const botReply = aiResponse(userText);
        addMessage(botReply, 'bot');
    }, 500);
}

chatSend.addEventListener('click', sendMessage);
chatInput.addEventListener('keypress', (e)=>{
    if(e.key === 'Enter'){
        sendMessage();
    }
});
</script>

</body>
</html>
