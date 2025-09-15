<h1 align="center">🚀 Allan Kelven - Full Stack Developer 🛠️</h1>

<p align="center">
  Criando soluções digitais inteligentes com <strong>8+ anos de experiência</strong>.
</p>

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:000428,100:004e92&height=200&section=header&text=Allan%20Kelven&fontColor=00e0ff&fontSize=40&animation=fadeIn" />
</div>

<div align="center">
  <a href="https://github.com/allankdev">
    <img height="180em" src="https://github-readme-stats.vercel.app/api?username=allankdev&show_icons=true&theme=github_dark&hide_border=true&include_all_commits=true&count_private=true&title_color=00e0ff&icon_color=00e0ff&text_color=c3c3c3&bg_color=0d0d0d"/>
    <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=allankdev&layout=compact&langs_count=8&theme=github_dark&hide_border=true&title_color=00e0ff&text_color=c3c3c3&bg_color=0d0d0d"/>
  </a>
</div>

---

## 🛠️ Tech Stack

<div align="center">
  <img src="https://img.shields.io/badge/JavaScript-0d0d0d?style=for-the-badge&logo=javascript&logoColor=00e0ff" />
  <img src="https://img.shields.io/badge/TypeScript-0d0d0d?style=for-the-badge&logo=typescript&logoColor=007acc" />
  <img src="https://img.shields.io/badge/React-0d0d0d?style=for-the-badge&logo=react&logoColor=61dafb" />
  <img src="https://img.shields.io/badge/Next.js-0d0d0d?style=for-the-badge&logo=nextdotjs&logoColor=ffffff" />
  <img src="https://img.shields.io/badge/Spring%20Boot-0d0d0d?style=for-the-badge&logo=spring-boot&logoColor=6db33f" />
  <img src="https://img.shields.io/badge/Node.js-0d0d0d?style=for-the-badge&logo=node.js&logoColor=00ff00" />
  <img src="https://img.shields.io/badge/Python-0d0d0d?style=for-the-badge&logo=python&logoColor=ffdd54" />
  <img src="https://img.shields.io/badge/Docker-0d0d0d?style=for-the-badge&logo=docker&logoColor=2496ed" />
</div>

---

## ⚙️ Sobre Mim

- 💼 Fundador da **Pethost** e **Meu Site BR**
- 🛠️ +8 anos entregando soluções escaláveis em **Java, React, Node.js e Python**
- 🚀 Experiência em **arquitetura de microserviços, automação e integrações**
- 💡 Filosofia: *Ou você domina a IA, ou será dominado por ela.*
- 🖤 Minimalista por essência

---

## 🌟 Projetos em Destaque

- 🐾 [**Pethost**](https://github.com/co-finampy/pethost-web.git) – Plataforma completa de hospedagem para pets  
- 📦 [**Pedego**](https://github.com/allankdev/pedego-api.git) – Sistema de entregas com API escalável  
- 👨‍💼 [**HR Contábil**](https://github.com/allankdev/hr-contabil.git) – Gestão de RH para contabilidades  
- 📰 [**Plataforma de Notícias**](https://github.com/allankdev/frontend-news.git) – Atualizações em tempo real  
- 🤖 [**Bot SMS Telegram**](https://github.com/allankdev/botsms.git) – Automação de atendimento via SMS

---

## 🌐 Redes Sociais

<div align="center">
  <a href="https://instagram.com/kelvenallan" target="_blank"><img src="https://img.shields.io/badge/-Instagram-0d0d0d?style=for-the-badge&logo=instagram&logoColor=00e0ff"></a>
  <a href="mailto:allankelven.ak@gmail.com"><img src="https://img.shields.io/badge/-Gmail-0d0d0d?style=for-the-badge&logo=gmail&logoColor=d32f2f"></a>
  <a href="https://www.linkedin.com/in/allankelven" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-0d0d0d?style=for-the-badge&logo=linkedin&logoColor=0e76a8"></a>
  <a href="https://discord.com/users/allankelven92" target="_blank"><img src="https://img.shields.io/badge/Discord-0d0d0d?style=for-the-badge&logo=discord&logoColor=7289da"></a>
</div>

---

## 📊 Atividade Recente

<div align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=allankdev&bg_color=0d0d0d&color=c3c3c3&line=00e0ff&point=00ff00&hide_border=true" />
</div>

---

## 🎮 Mini Game: Snake 🐍

> Abra o README no navegador com extensão **Markdown Preview** e jogue!

```html
<canvas id="snake" width="300" height="300" style="border:1px solid #00e0ff;"></canvas>
<script>
const canvas=document.getElementById("snake"),ctx=canvas.getContext("2d");
let box=15,snake=[{x:9*box,y:9*box}],dir,food={x:Math.floor(Math.random()*20)*box,y:Math.floor(Math.random()*20)*box};
document.addEventListener("keydown",e=>{if(e.keyCode==37&&dir!="right")dir="left";if(e.keyCode==38&&dir!="down")dir="up";if(e.keyCode==39&&dir!="left")dir="right";if(e.keyCode==40&&dir!="up")dir="down";});
function draw(){
  ctx.fillStyle="#0d0d0d";ctx.fillRect(0,0,300,300);
  for(let i=0;i<snake.length;i++){ctx.fillStyle=i==0?"#00e0ff":"#c3c3c3";ctx.fillRect(snake[i].x,snake[i].y,box,box);}
  ctx.fillStyle="#ff0000";ctx.fillRect(food.x,food.y,box,box);
  let snakeX=snake[0].x,snakeY=snake[0].y;
  if(dir=="left")snakeX-=box;if(dir=="up")snakeY-=box;if(dir=="right")snakeX+=box;if(dir=="down")snakeY+=box;
  if(snakeX==food.x&&snakeY==food.y){food={x:Math.floor(Math.random()*20)*box,y:Math.floor(Math.random()*20)*box};}
  else{snake.pop();}
  let newHead={x:snakeX,y:snakeY};
  if(snakeX<0||snakeY<0||snakeX>=300||snakeY>=300||snake.some(p=>p.x==newHead.x&&p.y==newHead.y)){clearInterval(game);}
  snake.unshift(newHead);
}
let game=setInterval(draw,100);
</script>
