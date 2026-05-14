# language-learning-website
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Language Learning Website</title>

  <style>
    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      font-family:Arial, sans-serif;
    }

    body{
      background:#f4f4f4;
      color:#333;
    }

    header{
      background:#4a90e2;
      color:white;
      padding:20px;
      text-align:center;
    }

    nav{
      margin-top:10px;
    }

    nav a{
      color:white;
      text-decoration:none;
      margin:0 15px;
      font-weight:bold;
    }

    .hero{
      text-align:center;
      padding:80px 20px;
      background:linear-gradient(to right,#4a90e2,#6dd5fa);
      color:white;
    }

    .hero button{
      margin-top:20px;
      padding:10px 20px;
      border:none;
      border-radius:5px;
      background:white;
      color:#4a90e2;
      cursor:pointer;
      font-size:16px;
    }

    .languages{
      padding:50px 20px;
      text-align:center;
    }

    .cards{
      display:flex;
      justify-content:center;
      flex-wrap:wrap;
      gap:20px;
      margin-top:20px;
    }

    .card{
      background:white;
      width:250px;
      padding:20px;
      border-radius:10px;
      box-shadow:0 2px 10px rgba(0,0,0,0.1);
    }

    .quiz{
      text-align:center;
      padding:50px 20px;
      background:white;
    }

    .quiz button{
      margin:10px;
      padding:10px 20px;
      border:none;
      background:#4a90e2;
      color:white;
      border-radius:5px;
      cursor:pointer;
    }

    .developer{
      text-align:center;
      padding:40px 20px;
    }

    .developer-box{
      background:white;
      max-width:500px;
      margin:auto;
      padding:25px;
      border-radius:10px;
      box-shadow:0 2px 10px rgba(0,0,0,0.1);
    }

    footer{
      background:#222;
      color:white;
      text-align:center;
      padding:15px;
      margin-top:20px;
    }
  </style>
</head>

<body>

<header>
  <h1>LinguaLearn</h1>

  <nav>
    <a href="#">Home</a>
    <a href="#">Languages</a>
    <a href="#">Quiz</a>
    <a href="#">Developer</a>
  </nav>
</header>

<section class="hero">
  <h2>Learn Languages Easily</h2>
  <p>Start learning new languages in a fun and interactive way.</p>

  <button onclick="welcomeMessage()">
    Start Learning
  </button>
</section>

<section class="languages">
  <h2>Popular Languages</h2>

  <div class="cards">

    <div class="card">
      <h3>English</h3>
      <p>Learn grammar, speaking and vocabulary.</p>
    </div>

    <div class="card">
      <h3>Spanish</h3>
      <p>Learn common Spanish words and phrases.</p>
    </div>

    <div class="card">
      <h3>French</h3>
      <p>Practice French pronunciation and writing.</p>
    </div>

  </div>
</section>

<section class="quiz">
  <h2>Quick Quiz</h2>

  <p>What is the Spanish word for Hello?</p>

  <button onclick="checkAnswer('Hola')">Hola</button>
  <button onclick="checkAnswer('Bonjour')">Bonjour</button>
  <button onclick="checkAnswer('Hello')">Hello</button>

  <h3 id="result"></h3>
</section>

<section class="developer">

  <h2>Developer Details</h2>

  <div class="developer-box">

    <h3>Syed Sahil Akhtar Rana</h3>

    <p><b>Course:</b> BCA in Cybersecurity</p>

    <p><b>University:</b> Assam down town University</p>

    <p>
      This Language Learning Website is a college project 
      developed by me using HTML, CSS and JavaScript.
    </p>

  </div>

</section>

<footer>
  <p>
    © 2026 Language Learning Website | Made by Syed Sahil Akhtar Rana
  </p>
</footer>

<script>

  function welcomeMessage(){
    alert("Welcome to LinguaLearn!");
  }

  function checkAnswer(answer){

    let result = document.getElementById("result");

    if(answer === "Hola"){
      result.innerHTML = "Correct Answer!";
      result.style.color = "green";
    }

    else{
      result.innerHTML = "Wrong Answer!";
      result.style.color = "red";
    }
  }

</script>

</body>
</html>
