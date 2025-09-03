<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Marta Martin Rozkydana | Portafolio</title>
<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600&display=swap" rel="stylesheet">
<style>
* {margin:0; padding:0; box-sizing:border-box; font-family:'Montserrat', sans-serif;}
body {line-height:1.6; color:#333; scroll-behavior:smooth; background:#fff;}
header {background:#f5f5f5; padding:60px 20px; text-align:center;}
header h1 {font-size:2.5rem; margin-bottom:10px;}
header h2 {font-size:1.2rem; font-weight:400; color:#555;}

nav {position:fixed; top:0; width:100%; background:#fff; box-shadow:0 2px 5px rgba(0,0,0,0.1); padding:10px 20px; z-index:100;}
nav a {margin:0 15px; color:#333; text-decoration:none; font-weight:600;}
nav a:hover {color:#007acc;}

section {padding:80px 20px; max-width:1000px; margin:0 auto;}
section h2 {text-align:center; margin-bottom:40px; font-size:2rem; color:#007acc;}

.experience, .skills-list {display:grid; gap:20px;}
.card {background:#f9f9f9; padding:20px; border-radius:10px; box-shadow:0 2px 10px rgba(0,0,0,0.05);}
.job-title, .project-title {font-weight:600; color:#007acc; margin-bottom:10px;}
.job-role, .project-role {font-style:italic; margin-bottom:10px;}
.skills-list {display:flex; flex-wrap:wrap; gap:10px; justify-content:center;}
.skill {background:#007acc; color:#fff; padding:8px 15px; border-radius:20px; font-size:0.9rem;}

/* GALERÍA CON MODAL */
.gallery {display:grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap:20px;}
.gallery-item {cursor:pointer; border-radius:10px; overflow:hidden; position:relative;}
.gallery-item img {width:100%; height:100%; object-fit:cover; transition:transform 0.3s;}
.gallery-item:hover img {transform:scale(1.05);}

/* Modal */
.modal {display:none; position:fixed; z-index:200; left:0; top:0; width:100%; height:100%; overflow:auto; background:rgba(0,0,0,0.9);}
.modal-content {background:#fff; margin:5% auto; padding:20px; max-width:800px; border-radius:10px; position:relative;}
.close {color:#333; position:absolute; top:15px; right:20px; font-size:30px; font-weight:bold; cursor:pointer;}
.modal-content img {width:100%; height:auto; border-radius:10px; margin-bottom:15px;}

footer {background:#f5f5f5; padding:40px 20px; text-align:center; font-size:0.9rem; color:#555;}
@media(max-width:600px){header h1{font-size:2rem;} header h2{font-size:1rem;}}
</style>
</head>
<body>
<nav>
    <a href="#sobre-mi">Sobre mí</a>
    <a href="#experiencia">Experiencia</a>
    <a href="#proyectos">Proyectos</a>
    <a href="#habilidades">Habilidades</a>
    <a href="#contacto">Contacto</a>
</nav>

<header>
    <h1>Marta Martin Rozkydana</h1>
    <h2>Diseñadora de vestuario e ilustradora freelance</h2>
</header>

<section id="sobre-mi">
    <h2>Sobre mí</h2>
    <p>Soy diseñadora de vestuario e ilustradora freelance especializada en cine y artes visuales, creando y confeccionando personalmente cada pieza de vestuario. También tengo experiencia en diseño digital, ilustración a mano y pintura al óleo. Apasionada por combinar creatividad, investigación y técnicas artesanales, aporto autenticidad y estilo único a cada proyecto audiovisual.</p>
</section>

<section id="experiencia">
    <h2>Experiencia</h2>
    <div class="experience">
        <div class="card">
            <div class="job-title">Barreira Arte y Diseño</div>
            <div class="job-role">Vestuario - Mayo 2025</div>
            <p>Diseño del vestuario en colaboración con un equipo, aportando creatividad y autenticidad para recrear la estética del clásico cinematográfico <em>El gabinete del doctor Caligari</em>.</p>
        </div>
    </div>
</section>

<section id="proyectos">
    <h2>Proyectos</h2>
    <div class="gallery">
        <div class="gallery-item" data-title="Femení Singular" data-desc="Ayudante de vestuario: preparación del vestuario y colaboración con el equipo." data-img="images/femeni-singular.jpg">
            <img src="images/femeni-singular.jpg" alt="Femení Singular">
        </div>
        <div class="gallery-item" data-title="El dia que falté" data-desc="Ayudante de vestuario: compras, setting, preparación y logística del vestuario." data-img="images/el-dia-que-falte.jpg">
            <img src="images/el-dia-que-falte.jpg" alt="El dia que falté">
        </div>
        <div class="gallery-item" data-title="Luz Azul" data-desc="Jefa de vestuario: organización, mood boards, compras y ambientación del vestuario completo." data-img="images/luz-azul.jpg">
            <img src="images/luz-azul.jpg" alt="Luz Azul">
        </div>
        <div class="gallery-item" data-title="Trabajo final de máster: Drácula" data-desc="Diseño integral del vestuario del personaje, patronaje, confección y ambientación realizados totalmente sola." data-img="images/dracula.jpg">
            <img src="images/dracula.jpg" alt="Drácula">
        </div>
    </div>
</section>

<!-- Modal -->
<div id="modal" class="modal">
    <div class="modal-content">
        <span class="close">&times;</span>
        <h2 id="modal-title"></h2>
        <img id="modal-img" src="" alt="">
        <p id="modal-desc"></p>
    </div>
</div>

<section id="habilidades">
    <h2>Habilidades</h2>
    <div class="skills-list">
        <div class="skill">Diseño de vestuario</div>
        <div class="skill">Investigación de personajes</div>
        <div class="skill">Mood boards</div>
        <div class="skill">Patronaje</div>
        <div class="skill">Confección</div>
        <div class="skill">Fitting</div>
        <div class="skill">Ambientación</div>
        <div class="skill">Compras</div>
        <div class="skill">Logística de rodaje</div>
        <div class="skill">Supervisión de equipo</div>
        <div class="skill">Ilustración digital</div>
        <div class="skill">Ilustración a mano</div>
        <div class="skill">Pintura al óleo</div>
    </div>
</section>

<section id="contacto">
    <h2>Contacto</h2>
    <p>Email: <a href="mailto:tuemail@ejemplo.com">tuemail@ejemplo.com</a></p>
    <p>LinkedIn: <a href="https://www.linkedin.com" target="_blank">linkedin.com/in/tuusuario</a></p>
    <p>Portafolio: <a href="https://www.behance.net" target="_blank">behance.net/tuusuario</a></p>
</section>

<footer>
    &copy; 2025 Marta Martin Rozkydana. Todos los derechos reservados.
</footer>

<script>
const modal = document.getElementById('modal');
const modalImg = document.getElementById('modal-img');
const modalTitle = document.getElementById('modal-title');
const modalDesc = document.getElementById('modal-desc');
const closeBtn = document.querySelector('.close');

document.querySelectorAll('.gallery-item').forEach(item => {
    item.addEventListener('click', () => {
        modal.style.display = 'block';
        modalImg.src = item.getAttribute('data-img');
        modalTitle.textContent = item.getAttribute('data-title');
        modalDesc.textContent = item.getAttribute('data-desc');
    });
});

closeBtn.onclick = () => { modal.style.display = 'none'; }
window.onclick = e => { if(e.target == modal) modal.style.display = 'none'; }
</script>
</body>
</html>