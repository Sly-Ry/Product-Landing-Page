# Product-Landing-Page
Freecodeonline Project: A product landing page created using HTML and CSS

+ HTML

** start of undefined **

```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8"/>
    <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
    <title>Product Landing Page</title>
    <link rel="stylesheet" href="./styles.css"/>
  </head>
  <body>
    <div class="page-wrapper">
      <header id="header">
        <div class="logo">
          <img id="header-img" alt="logo" src="https://i.pinimg.com/originals/39/e9/a3/39e9a35f632f70edba3d2073bd885d01.jpg"/>
        </div>
        <nav id="nav-bar">
          <ul>
            <li>
              <a class="nav-link" href="#features">Features</a>
            </li>
            <li>
              <a class="nav-link" href="#media">Media</a>
            </li>
            <li>
              <a class="nav-link" href="#styles">Styles</a>
            </li>
          </ul>
        </nav>
      </header>
      <div class="container"></div>
      <section class="hero">
        <h2>PICKLERS' PICKLES</h2>
        <form id="form" action="https://www.freecodecamp.com/email-submit">
          <input 
            id="email" 
            type="email" 
            name="email" 
            placeholder="Enter your email address"
            required
          />
          <input id="submit" type="submit" value="Enter" class="btn"/>
        </form>
      </section>
      <div class="container">
        <section id="features">

        </section>
        <section id="media">
          <div class="video" id="recipe">
            <iframe id="video" height="315" src="https://www.youtube.com/embed/4BOCrlwFeHc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
          </div>
          <div class="video" id="recipe">
            <iframe height="315" src="https://www.youtube.com/embed/vD6XWXj9l8Q" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
          </div>
          <div class="video" id="how-to">
            <iframe height="315" src="https://www.youtube.com/embed/qu9BR0IyWZI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
          </div>
          
        </section>
        <section id="styles">
          <div class="style" id="whole">
            <div class="name">WHOLE</div>
            <div class="info">
              <h2 class="price-range">$5 - $30</h2>
              <ol class="brands-by-votes">
                <li>Vlasic</li>
                <li>Claussen</li>
                <li>Mt. Olive</li>
              </ol>
            </div>
            <button class="btn">P</button>
          </div>
          <div class="style" id="spears">
            <div class="name">SPEAR</div>
            <h2 class="price-range">$3 - $27</h2>
            <ol class="brands-by-votes">
              <li>Vlasic</li>
              <li>Claussen</li>
              <li>Mt. Olive</li>
            </ol>
            <button class="btn">P</button>
          </div>
          <div class="style" id="slices">
            <div class="name">SLICE</div>
            <h2 class="price-range">$2 - $10</h2>
            <ol class="brands-by-votes">
              <li>Vlasic</li>
              <li>Claussen</li>
              <li>Mt. Olive</li>
            </ol>
            <button class="btn">P</button>
          </div>
          </div>
        </section>
        <footer>
          <ul>
            <li>
              <a href="#">Privacy</a>
              </li>
            <li>
              <a href="#">Terms</a>
            </li>
            <li>
              <a href="#">Contact</a>
            </li>
          </ul>
          <span>Copyright 2023, Picklers' Pickles</span>
        </footer>
      </div>
    </div>
  </body>
</html>
```

** end of undefined **


+ CSS

** start of undefined **

```
/* global element styling */

@import 'https://fonts.googleapis.com/css?family=Lato:400,700';

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  display: block;
}

body {  
  font-family: 'Lato', sans-serif;
  background-color: rgba(90, 180, 70, .3);
}

.page-wrapper {
  position: relative;
}

li {
  list-style: none;
}

a {
  color: black;
  text-decoration: none;
}


/* global classes styling */

.container {
  width: 100%;
  margin: 0 auto;
}

.btn {
  font-size: .9em;
  cursor: pointer;
}


/* Header Section */
header {
  position: fixed;
  top: 0;
  width: 100%;
  min-height: 70px;
  padding: 0px 20px;
  display: flex;
  justify-content: space-around;
  align-items: center;
  background-color: rgb(86, 78, 64);
  border-bottom: 5px solid rgb(71, 105, 70);
  z-index: 1; 
}

@media (max-width: 500px) {
  header { 
    flex-wrap: wrap;
  }
}

.logo {
 width: 65vw;
}

@media (max-width: 500px) {
  .logo {
    margin-top: 15px;
    width: 100%;
    position: relative;
  }
}

.logo img {
  margin: 20px 0 10px 0;
  width: 100%;
  height: 80px;
  max-width: 150px;
  display: flex;
  align-items: center;
  text-align: center;
  justify-content: center;
  border-radius: 35% 55%;
  rotate: -9deg;
}

@media (max-width: 500px) {
  .logo img {
    margin: 0 auto;
  } 
}

nav {
  font-weight: 600;
}

@media (max-width: 500px) {
  nav {
    margin-top: 10px;
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    padding: 0 50px;
    transition: smooth;
  }
}

nav ul {
  width: 35vw;
  display: flex;
  flex-direction: row;
  justify-content: space-around;
}

nav ul li {
  list-style: none;
  
}

@media (max-width: 500px) {
  nav ul {
    flex-direction: column;
  }
}

/* Hero Section */
.hero {
  position: relative;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  height: 80%;
  width: auto;
  margin-top: 100px;
}

.hero::before {
  content: "";
  background-image: url("https://c4.wallpaperflare.com/wallpaper/463/878/519/pickles-vegetables-food-green-wallpaper-preview.jpg");
  opacity: .7;
  background-position: center;
  background-repeat: no-repeat;
  height: 100%;
  min-width: 100%;
  background-size: cover;
  position: absolute;
  z-index: -9999
}

.hero h2 {
  margin-bottom: 55px;
  padding: 15px;
  word-wrap: break-word;
  font-style: Lato, sans-serif;
  font-size: 500%;
  text-shadow: 1px 8px 7px rgb(0, 0, 0);
  color: rgb(53, 203, 161);
  border: 2px solid  rgba(100, 200, 150, .7);
}

@media (max-width: 500px){
  .hero {
    margin-top: 150px;
    height: 50%;
  }

  .hero h2 {
    font-size: 400%;
  }
}

form {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}

.hero input[type="email"] {
  max-width: 350px;
  width: 100%;
  padding: 10px;
  margin-right: 5px;
  margin-bottom: 10px;
  background-color: rgba(0, 0, 0, .7);
  border: 1px solid rgb(255, 255, 255, .5);
  font-size: 15px;
  color: white;
}

.hero input[type="submit"] {
  max-width: 70px;
  width: 100%;
  height: 30px;
  border: 3px solid rgb(58, 103, 67);
  border-radius: 13px;
  background-color: rgb(137, 173, 118);
  font-weight: bold;
  color: rgb(0, 0, 0);
}

.hero input[type="submit"]:hover {
  background-color: rgb(79, 215, 30);
  border: 3px solid rgb(177, 255, 193);
  color: rgb(255, 255, 255);
  transition: 
    background-color 1s, 
    border .5s,
    color .5s;
}


/* Features Section
#features {
  margin-top: 30px;
} */


/* Media Section */
#media {
  padding: 50px 0;
  display: flex;
  justify-content: center;
  background-color: rgba(0,0,0,.5);
  width: 100%;
}

#media .video {
  padding: 0 5px;
}

#media .video iframe {
  max-width: 530px;
  min-width: 270px;
  width: 100%;
  margin: 0;
  border-top: 20px solid rgb(195, 195, 65);
  border-radius: 0 0 20px 20px;
  box-shadow:  0px 5px 10px black;
}


/* Styles Section */
#styles {
  margin-top: 50px;
  display: flex;
  flex-direction: row;
  justify-content: center;
}

#styles .style {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  width: calc(100% / 3);
  min-width: 160px;
  margin: 10px;
  border: 1px solid black;
  border-radius: 4px;
  overflow: hidden;
}

.name {
  background-color: rgb(45, 57, 9);
  color: white;
  padding: 10px 0;
  font-weight: 700;
  width: 100%;
  text-transform: uppercase;
}

.price-range {
  margin-top: 7px;
  font-style: italic;
}

.brands-by-votes {
  margin: 15px 0;
}

.style .btn {
  margin: -5px 0 10px 0;
  max-width: 40px;
  width: 100%;
  height: 30px;
  border: 3px solid rgb(58, 103, 67);
  border-radius: 13px;
  background-color: rgb(137, 173, 118);
  font-weight: bold;
  color: rgb(0, 0, 0);
}

.style .btn:hover {
 background-color: rgb(79, 215, 30);
 border: 3px solid rgb(177, 255, 193);
 color: rgb(255, 255, 255);
 transition: 
  background-color 1s, 
  border .5s,
  color .5s; 
}

@media (max-width: 650px) {
  #styles {
    flex-direction: column;
    align-items: center;
  }
  .style {
    max-width: 300px;
    width: 100%;
    margin: 0 auto;
    margin-bottom: 10px;
  }
}


/* Footer */
footer {
  margin-top: 50px;
  background-color: rgb(162, 158, 137);
  padding: 15px;
}

footer ul {
  display: flex;
  justify-content: flex-end;
}

footer ul li {
  padding: 0 10px;
}

footer span {
  margin-top: 5px;
  display: flex;
  justify-content: flex-end;
  font-size: 0.9em;
  color: #444
}
```

** end of undefined **
