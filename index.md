---
layout: base
title: Student Home 
description: Home Page
hide: true
---

# Welcome to Sharon Kodali's Blog

## About Me

![Sharon Kodali1](/images/notebooks/foundation/IMG_2674.JPG)   

Hi! I'm Sharon Kodali, a passionate student with a love for technology, coding, and creative writing. This blog is my space to share thoughts, projects, and experiences as I navigate my journey through college and beyond. I believe in continuous learning, and I'm excited to explore and document my growth here. Outside of academics, I enjoy painting, hiking, and exploring new cuisines.

---

## Guess the Number Game

<p>Try to guess the number I'm thinking of between 1 and 100!</p>

<input type="number" id="guessInput" placeholder="Enter your guess">
<button id="guessButton">Guess</button>

<p id="result"></p>

<script>
  const randomNumber = Math.floor(Math.random() * 100) + 1;
  let attempts = 0;

  document.getElementById("guessButton").addEventListener("click", function() {
    const userGuess = parseInt(document.getElementById("guessInput").value);
    attempts++;

    let resultMessage = '';

    if (userGuess === randomNumber) {
      resultMessage = `Congratulations! You guessed the right number ${randomNumber} in ${attempts} attempts.`;
    } else if (userGuess < randomNumber) {
      resultMessage = "Too low! Try again.";
    } else if (userGuess > randomNumber) {
      resultMessage = "Too high! Try again.";
    }

    document.getElementById("result").innerText = resultMessage;
  });
</script>

---

![Shar](/images/notebooks/foundation/IMG_1185%202.png)  
![Sh](/images/notebooks/foundation/IMG_2776.JPG)
![li](/images/notebooks/foundation/IMG_6016.JPG)
![S](/images/notebooks/foundation/IMG_7198.JPG)

Thank you for visiting! Stay tuned for more updates and posts.

<style>
  @import url('https://fonts.googleapis.com/css2?family=Press+Start+2P&display=swap');

  body {
    font-family: 'Press Start 2P', cursive;
    background-color: #f5f5f5;
    color: #333;
    line-height: 1.6;
    padding: 20px;
  }

  h1 {
    color: #ff6347;
    text-align: center;
    font-size: 2.5em;
    margin-top: 20px;
  }

  h2 {
    color: #87cefa;
    font-size: 2em;
    text-align: center;
    margin-top: 20px;
  }

  img {
    display: block;
    margin: 0 auto;
    border-radius: 50%;
    max-width: 150px;
    margin-top: 15px;
  }

  p {
    font-size: 1.2em;
    text-align: center;
    padding: 0 20px;
  }

  .content {
    background-color: #fff;
    border-radius: 8px;
    padding: 20px;
    margin: 20px auto;
    max-width: 800px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  }

  .footer {
    text-align: center;
    background-color: #333;
    color: #fff;
    padding: 10px;
    border-radius: 8px;
    margin-top: 40px;
  }

  input, button {
    display: block;
    margin: 10px auto;
    padding: 10px;
    font-size: 1.2em;
  }

  button {
    background-color: #87cefa;
    color: #fff;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
    transition: background-color 0.3s ease;
  }

  button:hover {
    background-color: #ff6347;
  }

  #result {
    font-size: 1.2em;
    text-align: center;
    margin-top: 20px;
  }
</style>


