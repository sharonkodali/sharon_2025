---
layout: base
title: Student Home
description: Home Page
hide: true
---

# Welcome to Sharon Kodali's Blog

## About Me

<div class="about-section">
  <img src="/images/notebooks/foundation/IMG_2674.JPG" alt="Sharon Kodali" class="profile-pic">
  <p>Hi, my name is Sharon! I love cooking and socializing. I enjoy going to the beach and driving around with my friends.</p>
</div>

# Things I need to work on and feedback from teacher 
<ul>
  <li>Write more detailed explanations</li>
  <li>Improve formatting consistency</li>
  <li>Engage more with content feedback</li>
</ul>

---

## Guess the Number Game

<p>Try to guess the number I'm thinking of between 1 and 100!</p>

<div class="game-section">
  <input type="number" id="guessInput" placeholder="Enter your guess">
  <button id="guessButton">Guess</button>
  <p id="result"></p>
</div>

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

<div class="photo-gallery">
  <img src="/images/notebooks/foundation/IMG_1185%202.png" alt="Gallery Image 1">
  <img src="/images/notebooks/foundation/IMG_2776.JPG" alt="Gallery Image 2">
  <img src="/images/notebooks/foundation/IMG_6016.JPG" alt="Gallery Image 3">
  <img src="/images/notebooks/foundation/IMG_7198.JPG" alt="Gallery Image 4">
</div>

<div class="footer">
  <p>Thank you for visiting! Stay tuned for more updates and posts.</p>
</div>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Press+Start+2P&display=swap');

  body {
    font-family: 'Press Start 2P', cursive;
    background-color: #ffe6f2; /* Light pink background */
    color: #333;
    line-height: 1.6;
    padding: 20px;
  }

  h1 {
    color: #ff1493; /* Pink title */
    text-align: center;
    font-size: 2.5em;
    margin-top: 20px;
  }

  h2 {
    color: #ff69b4;
    font-size: 2em;
    text-align: center;
    margin-top: 20px;
  }

  .about-section {
    text-align: center;
    max-width: 800px;
    margin: 0 auto;
  }

  .profile-pic {
    display: block;
    margin: 0 auto;
    border-radius: 50%;
    max-width: 150px;
    margin-top: 15px;
  }

  p {
    font-size: 1.2em;
    text-align: center;
  }

  .game-section {
    text-align: center;
    margin-top: 20px;
  }

  input, button {
    display: block;
    margin: 10px auto;
    padding: 10px;
    font-size: 1.2em;
    border-radius: 5px;
  }

  button {
    background-color: #ff69b4; /* Bright pink */
    color: #fff;
    border: none;
    cursor: pointer;
    transition: background-color 0.3s ease;
  }

  button:hover {
    background-color: #ff1493;
  }

  #result {
    font-size: 1.2em;
    margin-top: 20px;
  }

  .photo-gallery {
    display: flex;
    justify-content: center;
    gap: 10px;
    flex-wrap: wrap;
    margin-top: 20px;
  }

  .photo-gallery img {
    max-width: 150px;
    border-radius: 8px;
  }

  .footer {
    text-align: center;
    background-color: #ff1493;
    color: #fff;
    padding: 15px;
    margin-top: 30px;
    border-radius: 8px;
  }

  ul {
    text-align: left;
    max-width: 800px;
    margin: 0 auto;
    font-size: 1.1em;
    list-style-type: disc;
    padding-left: 20px;
  }
</style>



