---
layout: base
title: Student Home
description: Home Page
hide: true
---

# Welcome to Sharon Kodali's Blog

## About Me

<div class="about-section">
  <p>Hi, my name is Sharon! I love cooking and socializing. I enjoy going to the beach and driving around with my friends.</p>
</div>

# Things I need to work on and feedback from teacher
<ul>
  <li>Write more detailed explanations</li>
  <li>Improve formatting consistency</li>
  <li>Engage more with content feedback</li>
</ul>

---

## My Favorite Books Gallery

<p>Here are some of my favorite books:</p>

<div id="bookGallery" class="book-gallery"></div>

<script>
  // Array of favorite book ISBNs
  const favoriteBooks = [
    "9780143127741", // Example: "The Goldfinch"
    "9780679783268", // Example: "Pride and Prejudice"
    "9780743273565", // Example: "The Great Gatsby"
    "9780439139601", // Example: "Harry Potter and the Goblet of Fire"
    // Add more ISBNs of your favorite books
  ];

  const galleryContainer = document.getElementById('bookGallery');

  favoriteBooks.forEach(isbn => {
    // API endpoint to fetch book cover images
    const apiUrl = `https://covers.openlibrary.org/b/isbn/${isbn}-L.jpg`;
    
    // Create image element for each book
    const img = document.createElement('img');
    img.src = apiUrl;
    img.alt = "Book cover";
    img.className = 'book-cover';
    
    // Append image to gallery container
    galleryContainer.appendChild(img);
  });
</script>

---

<div class="footer">
  <p>Thank you for visiting! Stay tuned for more updates and posts.</p>
</div>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap');

  body {
    font-family: 'Poppins', sans-serif;
    background-color: #ffe4e1; /* Light pink background */
    color: #333;
    line-height: 1.6;
    padding: 20px;
    max-width: 1000px;
    margin: auto;
    text-align: center;
  }

  h1, h2 {
    color: #ff69b4; /* Pink color */
  }

  h1 {
    font-size: 2.5em;
    margin-top: 20px;
  }

  h2 {
    font-size: 2em;
    margin-top: 20px;
  }

  .about-section {
    text-align: center;
    max-width: 800px;
    margin: 0 auto;
  }

  p {
    font-size: 1.2em;
    color: #ff69b4;
  }

  ul {
    text-align: left;
    max-width: 800px;
    margin: 20px auto;
    font-size: 1.1em;
    list-style-type: disc;
    padding-left: 20px;
  }

  .book-gallery {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 20px;
    padding: 20px;
  }

  .book-cover {
    width: 150px;
    height: 225px;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    transition: transform 0.3s ease;
  }

  .book-cover:hover {
    transform: scale(1.05);
  }

  .footer {
    text-align: center;
    background-color: #ff69b4; /* Bright pink */
    color: #fff;
    padding: 15px;
    margin-top: 30px;
    border-radius: 8px;
  }
</style>




