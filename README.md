# Systema Araújo, redesign 3D

Redesign do site systemaaraujo.com.br (Systema, defesa pessoal russa, instrutor Rodrigo Araujo) com o material do próprio site, de um jeito mais interativo.

**Problema:** o site atual tem bastante conteúdo (canal com 96,9 mil inscritos, cards "54 Dias Mais Preparado", seminários, programa Embaixador), só que em páginas estáticas.

**Solução:** uma página única no conceito "Respiração":
- hero em WebGL com o urso num medalhão 3D e os cards orbitando, que se espalham com a rolagem;
- seção dos 4 elementos com um anel que inspira e expira junto com a rolagem (pin do GSAP);
- baralho de cards em leque;
- carrossel 3D dos shorts, que dá pra arrastar;
- questionário do Embaixador em 7 etapas, que envia pelo WhatsApp.

**Stack:** HTML/CSS/JS puro, Three.js 0.160, GSAP 3.12 + ScrollTrigger, Lenis. Sem build.

**Como rodar:** `python -m http.server 5215` na pasta e abrir http://127.0.0.1:5215/. Use http, não file://, porque alguns navegadores bloqueiam WebGL em arquivo local.
