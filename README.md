# Food-recipe
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Filipino Cuisine</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: #fffdd0;
      color: #333;
    }

    nav {
      background-color: #333;
      padding: 26px;
      text-align: center;
    }

    nav a {
      color: #fff;
      margin: 0 20px;
      cursor: pointer;
      text-decoration: none;
      font-weight: bold;
    }

    nav a:hover {
      color: #ffc107;
    }

    .page {
      display: none;
      padding: 20px;
    }

    .active {
      display: block;
    }

    .card {
      background-color: #ffffff;
      border-radius: 8px;
      padding: 15px;
      margin-bottom: 20px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
    }

    .card img {
      max-width: 100%;
      border-radius: 5px;
    }

    button {
      background-color: #ffc107;
      border: none;
      padding: 10px 15px;
      margin-top: 10px;
      cursor: pointer;
      border-radius: 5px;
      font-weight: bold;
    }

    button:hover {
      background-color: #e0a800;
    }

    h1 {
      text-align: center;
      padding: 40px 10px 10px;
      color: #f76d37;
      font-size: 3em;
      font-family: 'Georgia', serif;
    }

    .intro {
      text-align: center;
      padding: 10px 30px;
      font-size: 18px;
      color: #555;
      max-width: 700px;
      margin: auto;
    }

    .back-btn {
      margin-bottom: 20px;
    }

    .contact-info {
      text-align: center;
      padding: 40px;
      background-color: #fff;
      border-radius: 8px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
      max-width: 800px;
      margin: auto;
    }
    .menu-container {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  justify-content: center;
  padding: 20px;
}

.menu-container .card {
  flex: 2 2 300px;
  max-width: 300px;
}
form {
  display: flex;
  flex-direction: column;
}

form label {
  margin-top: 10px;
  font-weight: bold;
}

form input,
form textarea {
  padding: 10px;
  margin-top: 5px;
  border: 1px solid #ccc;
  border-radius: 5px;
  font-size: 16px;
  font-family: Arial, sans-serif;
}

form input:focus,
form textarea:focus {
  border-color: #1a73e8;
  outline: none;
}

form button {
  background-color: #1a73e8;
  color: white;
  border: none;
  margin-top: 15px;
  padding: 12px;
  border-radius: 5px;
  cursor: pointer;
  font-weight: bold;
}

form button:hover {
  background-color: #155ac3;
}


  </style>
  <script>
    function showPage(pageId) {
      document.querySelectorAll('.page').forEach(function (page) {
        page.classList.remove('active');
      });
      document.getElementById(pageId).classList.add('active');
    }

    window.onload = function () {
      showPage('homePage');
    }

  </script>
</head>
<body>

  <!-- Navigation -->
  <nav>
    <a onclick="showPage('homePage')">🏠Home</a> |
    <a onclick="showPage('menuPage')">🍽️ Menu</a> |
    <a onclick="showPage('contactPage')">📞 Contact</a>
  </nav>

  <!-- Home Page -->
  <div id="homePage" class="page active">
    <br><br><br><br><br><br><br><br>
    <h1><font-family></font-family>Filipino Cuisine</h1>
    <p class="intro">
      Welcome to the rich and flavorful world of Filipino cuisine.<br>
      Explore traditional dishes passed down through generations, filled with warmth and culture.
    </p>
  </div>

  <!-- Menu Page -->
  <div id="menuPage" class="page">
    <h2 style="text-align: center;">MENU</h2>
    <br><br><br><br>
    <div class="menu-container">
      <div class="card">
        <h3>Chicken Adobo</h3>
        <p>A savory dish with soy sauce, vinegar, garlic, and love.</p>
        <center>
        <img src="c:\Users\Asus\Desktop\p3 html\images\Classic Chicken Adobo.jpg" alt="Chicken Adobo" width="200">
        <button onclick="showPage('adoboPage')">View Chicken Adobo Recipe</button>
        </center>
      </div>
      <div class="card">
        <h3>Sinigang</h3>
        <p>Sour pork soup with tamarind and fresh vegetables.</p>
        <center>
        <img src="c:\Users\Asus\Desktop\p3 html\images\Sinigang na Baboy.jpg" alt="Sinigang" width="200">
        <button onclick="showPage('sinigangPage')">View Sinigang Recipe</button>
        </center>
      </div>
      <div class="card">
        <h3>Beef Caldereta</h3>
        <p>Hearty beef stew with tomato sauce, potatoes, carrots, and liver spread.</p>
        <center>
        <img src="c:\Users\Asus\Desktop\p3 html\images\Lainy’s Beef Caldereta Recipe.jpg" alt="Beef Caldereta" width="200">
        <button onclick="showPage('calderetaPage')">View Beef Caldereta Recipe</button>
        </center>
      </div>
    </div>
  </div>
  

  <!-- Chicken Adobo Page -->
  <div id="adoboPage" class="page">
    <button class="back-btn" onclick="showPage('menuPage')">← Back to Menu</button>
    <div class="card">
      <h3>Chicken Adobo</h3>
      <h4>Ingredients</h4>
      <ul>
        <li>1 tbsp canola oil</li>
        <li>4 chicken legs (thighs & drumsticks)</li>
        <li>Salt, garlic, bay leaves, black peppercorns</li>
        <li>1¼ cups water, 1 cup soy sauce, 1 cup rice vinegar</li>
        <li>Serve with steamed or garlic fried rice</li>
      </ul>
      <h4>How to Cook</h4>
    <ol>
      <li>Marinate chicken in soy sauce & vinegar.</li>
      <li>Sauté garlic, then add chicken and brown.</li>
      <li>Add marinade and simmer until tender.</li>
      <li>Serve with rice.</li>
    </ol>
    </div>
  </div>

  <!-- Sinigang Page -->
  <div id="sinigangPage" class="page">
    <button class="back-btn" onclick="showPage('menuPage')">← Back to Menu</button>
    <div class="card">
      <h3>Sinigang</h3>
      <h4>Ingredients</h4>
      <ul>
        <li>4¼ cups water, 2 cups pork ribs</li>
        <li>Onion, tomatoes, sitaw, kangkong</li>
        <li>Eggplant, chili, Sinigang mix</li>
        <li>Optional: labanos, okra</li>
      </ul>
      <h4>How to Cook</h4>
      <ol>
        <li>Boil pork in water.</li>
        <li>Add tamarind mix, tomatoes, onions.</li>
        <li>Simmer until pork is tender.</li>
        <li>Add vegetables, cook until soft.</li>
      </ol>
    </div>
  </div>

  <!-- Beef Caldereta Page -->
  <div id="calderetaPage" class="page">
    <button class="back-btn" onclick="showPage('menuPage')">← Back to Menu</button>
    <div class="card">
      <h3>Beef Caldereta</h3>
      <h4>Ingredients</h4>
      <ul>
        <li>2 lbs beef, onion, garlic</li>
        <li>Tomato sauce, liver spread</li>
        <li>Potatoes, carrots, bell peppers</li>
        <li>Salt, pepper, beef broth</li>
      </ul>
      <h4>How to Cook</h4>
      <ol>
        <li>Brown beef in oil.</li>
        <li>Add liver spread, tomato sauce, broth.</li>
        <li>Simmer until beef is tender.</li>
        <li>Add veggies and finish cooking.</li>
      </ol>
    </div>
    </div>
  </div>

  <!-- Contact Page -->
  <div id="contactPage" class="page">
    <div class="contact-info">
    <h2>Contact Us</h2>
    <div class="card" style="max-width: 400px; margin: 0 auto;">
      <form>
        <label for="name">Full Name</label>
        <input type="text" id="name" name="name" required>
  
        <label for="email">Gmail Address</label>
        <input type="email" id="email" name="email" placeholder="example@gmail.com" required>
  
        <label for="message">Message</label>
        <textarea id="message" name="message" rows="5" required></textarea>
  
        <button type="submit">Send Message</button>
      </form>
    </div>
  </div>
  <footer>
        <div class="footer-content">
            <center>
          <p>Follow us on:</p>
          <a href="https://facebook.com" target="_blank"><img src="https://cdn-icons-png.flaticon.com/512/733/733547.png" alt="Facebook" class="social-icon" width="30" height="30"></a>
          <a href="https://twitter.com" target="_blank"><img src="https://freepnglogo.com/images/all_img/1707222563twitter-logo-png.png" alt="X (formerly Twitter)" class="social-icon" width="30" height="30"></a>
          <a href="https://instagram.com" target="_blank"><img src="https://cdn-icons-png.flaticon.com/512/733/733558.png" alt="Instagram" class="social-icon" width="30" height="30"></a>
          <p>&copy; 2025 Filipino Cuisine</p>
          </center>
        </div>
      
    </footer>
</body>
</html>
