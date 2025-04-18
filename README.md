<div align="center">
  <style>
    /* Estilos globales */
    body {
      background-color: #0d1117;
      background-image: 
        radial-gradient(circle at 25% 25%, rgba(125, 137, 232, 0.15) 0%, transparent 40%),
        radial-gradient(circle at 75% 75%, rgba(78, 81, 238, 0.1) 0%, transparent 40%);
      background-attachment: fixed;
    }
    
    /* Animación de título */
    @keyframes gradientText {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }
    
    .gradient-title {
      background: linear-gradient(90deg, #8A2BE2, #4169E1, #9370DB, #6A5ACD);
      background-size: 300% 300%;
      animation: gradientText 6s ease infinite;
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      font-weight: 700;
      font-size: 2.5em;
      margin-bottom: 10px;
    }
    
    /* Tarjetas con efecto hover */
    .project-card {
      border-radius: 10px;
      overflow: hidden;
      transition: all 0.3s ease;
      border: 1px solid rgba(138, 43, 226, 0.2);
      box-shadow: 0 4px 20px rgba(138, 43, 226, 0.1);
    }
    
    .project-card:hover {
      transform: translateY(-5px);
      box-shadow: 0 10px 25px rgba(138, 43, 226, 0.2);
      border: 1px solid rgba(138, 43, 226, 0.5);
    }
    
    /* Badges personalizados */
    .custom-badge {
      display: inline-block;
      padding: 8px 16px;
      border-radius: 20px;
      font-weight: 600;
      margin: 5px;
      transition: all 0.3s ease;
      background: linear-gradient(90deg, #8A2BE2, #4169E1);
      color: white;
      box-shadow: 0 4px 10px rgba(138, 43, 226, 0.3);
    }
    
    .custom-badge:hover {
      transform: scale(1.05);
      box-shadow: 0 6px 15px rgba(138, 43, 226, 0.4);
    }
    
    /* Separadores animados */
    .animated-divider {
      height: 3px;
      background: linear-gradient(90deg, transparent, #8A2BE2, #4169E1, transparent);
      margin: 30px 0;
      position: relative;
      overflow: hidden;
    }
    
    .animated-divider::before {
      content: '';
      position: absolute;
      width: 100%;
      height: 100%;
      background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.8), transparent);
      transform: translateX(-100%);
      animation: dividerShine 3s infinite;
    }
    
    @keyframes dividerShine {
      100% { transform: translateX(100%); }
    }
    
    /* Animación de pulsación para iconos */
    @keyframes pulse {
      0% { transform: scale(1); }
      50% { transform: scale(1.1); }
      100% { transform: scale(1); }
    }
    
    .social-icon:hover {
      animation: pulse 1s infinite;
    }
    
    /* Fondo animado para secciones */
    .section-bg {
      position: relative;
      z-index: 1;
      padding: 20px;
      border-radius: 15px;
      background: rgba(13, 17, 23, 0.7);
      backdrop-filter: blur(5px);
      border: 1px solid rgba(138, 43, 226, 0.2);
    }
    
    /* SVG animado para decoración */
    .animated-circles {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      overflow: hidden;
      z-index: -1;
    }
  </style>
  
  <!-- SVG animado para el fondo -->
  <svg class="animated-circles" width="100%" height="100%" viewBox="0 0 1000 1000" xmlns="http://www.w3.org/2000/svg">
    <defs>
      <linearGradient id="grad1" x1="0%" y1="0%" x2="100%" y2="0%">
        <stop offset="0%" style="stop-color:#8A2BE2;stop-opacity:0.3" />
        <stop offset="100%" style="stop-color:#4169E1;stop-opacity:0.3" />
      </linearGradient>
    </defs>
    <circle cx="500" cy="500" r="300" fill="none" stroke="url(#grad1)" stroke-width="2">
      <animate attributeName="r" from="300" to="310" dur="4s" repeatCount="indefinite" />
      <animate attributeName="stroke-opacity" from="0.3" to="0.1" dur="4s" repeatCount="indefinite" />
    </circle>
    <circle cx="500" cy="500" r="250" fill="none" stroke="url(#grad1)" stroke-width="2">
      <animate attributeName="r" from="250" to="260" dur="5s" repeatCount="indefinite" />
      <animate attributeName="stroke-opacity" from="0.3" to="0.1" dur="5s" repeatCount="indefinite" />
    </circle>
    <circle cx="500" cy="500" r="200" fill="none" stroke="url(#grad1)" stroke-width="2">
      <animate attributeName="r" from="200" to="210" dur="6s" repeatCount="indefinite" />
      <animate attributeName="stroke-opacity" from="0.3" to="0.1" dur="6s" repeatCount="indefinite" />
    </circle>
  </svg>
  
  <h1 class="gradient-title">Hola, soy Jose Rico 👋</h1>
</div>

<div align="center" class="section-bg">
  <img src="https://drive.google.com/uc?export=view&id=1BNHtR0kNUSSO3wqMbOQ486qmrZ-fpkJI" 
       alt="Imagen de bienvenida" 
       style="display: block; margin: 0 auto; border-radius: 15px; max-width: 80%; box-shadow: 0 10px 30px rgba(138, 43, 226, 0.3); transition: transform 0.3s ease;" 
       onmouseover="this.style.transform='scale(1.02)'" 
       onmouseout="this.style.transform='scale(1)'">
</div>

<div align="center" style="margin-top: 20px;">
  <a href="https://www.instagram.com/richoflucky/profilecard/?igsh=MTh6ZmtxeDR1d2x3eA==" class="social-icon" style="margin: 0 10px;">
    <img src="https://img.shields.io/badge/-Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white" alt="Instagram">
  </a>
  <a href="https://www.facebook.com/richoflucky?mibextid=ZbWKwL" class="social-icon" style="margin: 0 10px;">
    <img src="https://img.shields.io/badge/-Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white" alt="Facebook">
  </a>
  <a href="https://discord.com/users/joserico_" class="social-icon" style="margin: 0 10px;">
    <img src="https://img.shields.io/badge/-Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord">
  </a>
  <a href="https://discord.gg/REqSYkHg" class="social-icon" style="margin: 0 10px;">
    <img src="https://img.shields.io/badge/-Join%20my%20Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Join Discord">
  </a>
</div>

<div class="section-bg" style="margin-top: 30px; padding: 25px;">
  <h2 style="color: #8A2BE2; border-bottom: 2px solid #4169E1; padding-bottom: 10px;">Sobre mí</h2>

  <ul style="list-style-type: none; padding-left: 10px;">
    <li style="margin: 15px 0; display: flex; align-items: center;">
      <span style="background: linear-gradient(90deg, #8A2BE2, #4169E1); -webkit-background-clip: text; -webkit-text-fill-color: transparent; font-size: 1.5em; margin-right: 10px;">📚</span> 
      Actualmente estoy aprendiendo a programar y me apasiona compartir mis conocimientos.
    </li>
    <li style="margin: 15px 0; display: flex; align-items: center;">
      <span style="background: linear-gradient(90deg, #8A2BE2, #4169E1); -webkit-background-clip: text; -webkit-text-fill-color: transparent; font-size: 1.5em; margin-right: 10px;">💻</span> 
      Mi lenguaje favorito es <strong style="color: #8A2BE2;">Python</strong>, pero también trabajo con <strong style="color: #4169E1;">C#</strong> y <strong style="color: #9370DB;">Java</strong>.
    </li>
    <li style="margin: 15px 0; display: flex; align-items: center;">
      <span style="background: linear-gradient(90deg, #8A2BE2, #4169E1); -webkit-background-clip: text; -webkit-text-fill-color: transparent; font-size: 1.5em; margin-right: 10px;">🚀</span> 
      Trabajo en proyectos pequeños para mejorar mis habilidades en desarrollo de software, además de conocer y trabajar con bases de datos como <strong style="color: #47A248;">MongoDB</strong> y <strong style="color: #4479A1;">MySQL</strong>.
    </li>
  </ul>
</div>

<div class="animated-divider"></div>

<div class="section-bg">
  <h2 style="color: #8A2BE2; border-bottom: 2px solid #4169E1; padding-bottom: 10px;">Proyectos destacados 🚀</h2>
  
  <table class="project-card" style="width: 100%; border-collapse: separate; border-spacing: 0;">
    <tr>
      <td style="padding: 20px; background: rgba(13, 17, 23, 0.5);">
        <h3 align="center" style="color: #8A2BE2;">Mi primer proyecto</h3>
        <div align="center">
          <a href="https://github.com/RMJGLUCKY27/DEAD_CELLS-DATABASE" target="_blank">
            <img src="https://i.ytimg.com/vi/vYVy0LwaC4E/maxresdefault.jpg" alt="Imagen de proyecto" width="400" style="border-radius: 10px; transition: transform 0.3s ease; box-shadow: 0 5px 15px rgba(138, 43, 226, 0.3);" onmouseover="this.style.transform='scale(1.03)'" onmouseout="this.style.transform='scale(1)'">
          </a>
          <p style="margin-top: 15px;">
            <a href="https://github.com/RMJGLUCKY27/DEAD_CELLS-DATABASE" target="_blank" style="text-decoration: none;">
              <span class="custom-badge">CÓDIGO</span>
            </a>
          </p>
          <p style="color: #e6e6e6;">Este proyecto es una base de datos para gestionar información relacionada con personajes, enemigos, niveles y objetos del videojuego Dead Cells.</p>
        </div>
      </td>
    </tr>
  </table>
</div>

<div class="animated-divider"></div>

<div class="section-bg">
  <h2 style="color: #8A2BE2; border-bottom: 2px solid #4169E1; padding-bottom: 10px;">Tecnologías y Lenguajes de Programación 🚀</h2>
  
  <div align="center" style="display: flex; flex-wrap: wrap; justify-content: center; gap: 15px; margin-top: 20px;">
    <div class="custom-badge" style="background: linear-gradient(90deg, #3776AB, #2b5c84);">Python</div>
    <div class="custom-badge" style="background: linear-gradient(90deg, #2396ED, #1a70b1);">C#</div>
    <div class="custom-badge" style="background: linear-gradient(90deg, #007396, #005571);">Java</div>
    <div class="custom-badge" style="background: linear-gradient(90deg, #47A248, #368136);">MongoDB</div>
    <div class="custom-badge" style="background: linear-gradient(90deg, #4479A1, #335f78);">MySQL</div>
  </div>
</div>

<div class="animated-divider"></div>

<div class="section-bg">
  <h2 style="color: #8A2BE2; border-bottom: 2px solid #4169E1; padding-bottom: 10px;">⚙️ &nbsp;GitHub Analytics</h2>
  
  <p align="center">
    <a href="https://github.com/RMJGLUCKY27">
      <img height="180em" src="https://github-readme-stats-eight-theta.vercel.app/api?username=RMJGLUCKY27&show_icons=true&theme=algolia&include_all_commits=true&count_private=true" style="margin: 10px; border-radius: 10px; box-shadow: 0 5px 15px rgba(138, 43, 226, 0.3); transition: transform 0.3s ease;" onmouseover="this.style.transform='scale(1.03)'" onmouseout="this.style.transform='scale(1)'">
      <img height="180em" src="https://github-readme-stats-eight-theta.vercel.app/api/top-langs/?username=RMJGLUCKY27&layout=compact&langs_count=8&theme=algolia" style="margin: 10px; border-radius: 10px; box-shadow: 0 5px 15px rgba(138, 43, 226, 0.3); transition: transform 0.3s ease;" onmouseover="this.style.transform='scale(1.03)'" onmouseout="this.style.transform='scale(1)'">
    </a>
  </p>
</div>

<!-- Animación de partículas flotantes -->
<svg width="0" height="0">
  <filter id="gooey">
    <feGaussianBlur in="SourceGraphic" stdDeviation="10" result="blur" />
    <feColorMatrix in="blur" mode="matrix" values="1 0 0 0 0  0 1 0 0 0  0 0 1 0 0  0 0 0 19 -9" result="goo" />
  </filter>
</svg>

<script>
  // Esta función se ejecutará cuando el README se cargue en GitHub
  document.addEventListener('DOMContentLoaded', function() {
    // Código para mejorar la experiencia visual si es necesario
    // GitHub sanitiza los scripts, pero dejamos esto como referencia
  });
</script>
