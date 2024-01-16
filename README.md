

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <script src="https://kit.fontawesome.com/f46ce87315.js" crossorigin="anonymous"></script>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/2.2.4/jquery.min.js"></script>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet"
        integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3"
        crossorigin="anonymous">
</head>
<!--- Present -->
<style type="text/css">
  .portada {
  background: url(https://i.pinimg.com/originals/7b/6f/05/7b6f055f5039f0f5646b961411e588b3.gif)
   no-repeat center center fixed;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
  width: 100%;
  height: 100vh;
  padding: 10%;
  margin-bottom: -10%;
}
@keyframes fadeInAndMoveUp {
  from {
    opacity: 0;
    transform: translateY(50%); /* Empieza 20px más abajo */
  }
  to {
    opacity: 1;
    transform: translateY(0); /* Llega a su posición original */
  }
}
.party {
    justify-content: center;
    align-items: center;
}
.logo{
    width:20%;
    height:auto;
    border-radius:100%;
}
.paradox {
  margin-top: 8%;
  text-align: center;
  font: 6em sans-serif;
  opacity: 0; /* Inicialmente oculto */
  animation: fadeInAndMoveUp 1s ease-in-out forwards; /* La animación de entrada y cambio de posición dura 2 segundos */
}

</style>
    <article class="portada">
      <div class="party">
        <h1 class="paradox" style="color:#FFF">
                  <img class="logo" src="data:image/png;base64,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">
            OsdroiX
        </h1>
      </div>
    </article>
          <!--horizontal divider(gradiant)-->
          <img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">

<!--- snake -->
<div align="center">
  <img  src="https://github.com/1999AZZAR/1999AZZAR/blob/main/resources/img/grid-snake.svg"
       alt="snake" /></a>
</div>


<!--h2 without bottom border-->
<div id="user-content-toc">
  <ul align="center">
    <summary><h2 style="display: inline-block">Confusion is part of Programming</h2></summary>
  </ul>
</div>


<!--Intro start-->
- 🔭 I’m currently working on **Java,Python, Nodejs,PHP,Mysql,,MongoDB**

- 🌱 I’m currently learning **to put together multiple Hyper Beast Stack for Scalable Applications.**

- ☁️ I've keen interest in cloud computing. So,I'm learning **AWS**

- 📝 I regularly write articles on [Hashnode](https://1010nishant.hashnode.dev/)

- 💬 Ask me about **AWS, react, react-native, nodejs, mongoDB**

- 📫 Feel free to reach me out **nishantjangid6377@gmail.com**

- 🏠 Also We've a tech community called [Dev Hac](https://discord.com/invite/p4TWyft886).
<!--Intro end-->



<!--- stats & Trophy (start) -->
<p align="center">
  <!--- stats (start) -->
<table align="center">
<tr border="none">
<td width="50%" align="center">
  
  <img  align="center"  src="https://github-readme-stats.vercel.app/api?username=osdroix&theme=dark&show_icons=true&count_private=true" />
  <br></br>
  <img  title="🔥 Get streak stats for your profile at git.io/streak-stats" alt="Mark streak" src="https://github-readme-streak-stats.herokuapp.com/?user=osdroix&theme=dark&hide_border=false" /> 
</td>

<td width="50%" align="center">

  <img  align="center"  src="https://github-readme-stats.anuraghazra1.vercel.app/api/top-langs/?username=osdroix&theme=dark&hide_border=false&no-bg=true&no-frame=true&langs_count=10"/>
  
  </td>
</tr>
</table>
<!--- stats (end) -->

</p>        
<!--- stats (end) -->


<!--h1 without bottom border-->
<div id="user-content-toc">
  <ul align="center">
    <summary><h2 style="display: inline-block">Technologies That I Know👨🏻‍💻</h2></summary>
  </ul>
</div>
<!--tech stack icons-->
<p align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=git,aws,bootstrap,c,cpp,css,discord,docker,dynamodb,express,figma,firebase,github,html,idea,java,js,kotlin,linux,md,materialui,mongodb,mysql,nextjs,nodejs,postman,py,react,redux,tailwind,ts,vscode&perline=14" />
  </a>
</p>


<!-- Connect with me -->
<!--h2 without bottom border-->
<div id="user-content-toc">
  <ul align="center">
    <summary><h2 style="display: inline-block">Connect With Me🤝</h2></summary>
  </ul>
</div>

<!--icons and links-->
<p align="center">
<a href="https://www.linkedin.com/in/1010nishant/" target="blank"><img align="center" src="https://user-images.githubusercontent.com/88904952/234979284-68c11d7f-1acc-4f0c-ac78-044e1037d7b0.png" alt="linkedin" height="50" width="50" /></a>
<a href="https://twitter.com/1010nishant" target="blank"><img align="center" src="https://user-images.githubusercontent.com/88904952/234980676-61bfb021-ecc8-48f7-88e6-34c1b06c4a58.png" alt="twitter" height="50" width="50" /></a> 
<a href="https://www.instagram.com/nishant.jangir.1010/" target="blank"><img align="center" src="https://user-images.githubusercontent.com/88904952/234981169-2dd1e58f-4b7e-468c-8213-034ba62156c3.png" alt="instagram" height="50" width="50" /></a>
<a href="https://1010nishant.hashnode.dev/" target="blank"><img align="center" src="https://user-images.githubusercontent.com/88904952/234982196-562aea17-5532-4550-8c08-1c7cb994a541.png" alt="hashnode" height="50" width="50" /></a>
<a href="https://discord.gg/UjwKkJsXsf" target="blank"><img align="center" src="https://user-images.githubusercontent.com/88904952/234982627-019fd336-6248-453c-9b05-97c13fd1d207.png" alt="discord" height="50" width="50" /></a>
  
</p>


<!--profile visit count-->
<div align="center">
  
[![](https://visitcount.itsvg.in/api?id=1010nishant&icon=3&color=6)](https://visitcount.itsvg.in)
  
</div>

<!--horizontal divider(gradiant)-->
<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">
