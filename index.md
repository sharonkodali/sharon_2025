---
---
layout: base
title: Sharon Kodali's Blog
description: Home Page
hide: false
---

# Welcome to Sharon Kodali's Blog

## About Me

<div class="about-section">
  <p>Hi, my name is Sharon Kodali! I’m passionate about technology, painting, and exploring new cuisines. I enjoy painting, hiking, and delving into various tech projects. Check out my latest projects and interests below!</p>

  <div class="image-gallery">
    <img src="_site/images/notebooks/foundation/IMG_2776.JPG" alt="Image 1">
    <img src="_site/images/notebooks/foundation/IMG_2777.JPG" alt="Image 2">
    <img src="_site/images/notebooks/foundation/IMG_2778.JPG" alt="Image 3">
  </div>
</div>

---

## Flags Gallery

<p>Here are some countries I've visited! (imported from wiki images):</p>

<div class="flag-gallery">
  <img src="https://upload.wikimedia.org/wikipedia/en/a/a4/Flag_of_India.svg" alt="India Flag" class="flag">
  <img src="https://upload.wikimedia.org/wikipedia/en/a/a4/Flag_of_the_United_States.svg" alt="USA Flag" class="flag">
  <img src="https://upload.wikimedia.org/wikipedia/en/0/03/Flag_of_Italy.svg" alt="Italy Flag" class="flag">
  <img src="https://upload.wikimedia.org/wikipedia/en/c/c3/Flag_of_France.svg" alt="France Flag" class="flag">
  <img src="https://upload.wikimedia.org/wikipedia/commons/f/f3/Flag_of_Switzerland.svg" alt="Switzerland Flag" class="flag">
  <img src="https://upload.wikimedia.org/wikipedia/commons/5/5c/Flag_of_Greece.svg" alt="Greece Flag" class="flag">
  <img src="https://upload.wikimedia.org/wikipedia/en/a/a4/Flag_of_the_United_Kingdom.svg" alt="UK Flag" class="flag">
  <img src="https://upload.wikimedia.org/wikipedia/commons/f/fc/Flag_of_Mexico.svg" alt="Mexico Flag" class="flag">
  <img src="https://upload.wikimedia.org/wikipedia/en/9/9e/Flag_of_Japan.svg" alt="Japan Flag" class="flag">
</div>

---

## My Favorite Books Gallery

<p>Ever since I was little, I have loved to read! Here are some of my favorite books:</p>

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

## Notebooks

<div class="notebook-menu">
  <ul>
    <li><a href="notebooks/planning.md">Planning Document</a></li>
    <li><a href="notebooks/javascript.md">JavaScript Notebook</a></li>
    <li><a href="notebooks/about.md">About Page Notebook</a></li>
  </ul>
</div>

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
    font-family: 'Poppins', sans-serif;
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

  .image-gallery {
    display: flex;
    justify-content: center;
    gap: 10px;
    padding: 20px;
  }

  .image-gallery img {
    width: 30%;
    height: auto;
    border-radius: 5px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
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

  .flag-gallery {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 10px;
    padding: 20px;
  }

  .flag {
    width: 64px;
    height: 64px;
    border-radius: 5px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
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

  .notebook-menu ul {
    list-style: none;
    padding: 0;
    font-size: 1.2em;
    margin: 0;
  }

  .notebook-menu li {
    margin: 10px 0;
  }

  .notebook-menu a {
    color: #ff69b4;
    text-decoration: none;
  }

  .notebook-menu a:hover {
    text-decoration: underline;
  }
</style>
