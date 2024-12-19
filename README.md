# Ex.07 Restaurant Website
## Date:19.12.2024

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
```
index.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Our Restaurant</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>Harshitha RESTAURANT</h1>
    <nav>
      <a href="about.html">About Us</a>
      <a href="menu.html">Menu</a>
      <a href="administration.html">Team</a>
      <a href="contact.html">Contact Us</a>
    </nav>
  </header>

  <section id="logo-details">
    <div class="logo-container">
      <img src="logo.jpeg" alt="Restaurant Logo" class="restaurant-logo">
    </div>
    <div class="restaurant-details">
      <h2>Welcome to Harshitha  Restaurant</h2>
      <p>Located in the heart of Chennai, Harshitha Restaurant offers a memorable dining experience with a focus on high-quality food and exceptional service. Our mission is to provide a wide variety of delicious dishes made from fresh, locally sourced ingredients in a warm and inviting atmosphere. Whether it's a casual meal or a special occasion, we have something for everyone!</p>
    </div>
  </section>

  <main>
    <section id="about">
        <h2>About Us</h2>
        <p>Learn more about our restaurant and the experience we offer to our customers. Click on the "About Us" link in the navigation to explore more.</p>
    </section>

  </main>

  <footer>
    <p>&copy; 2024 Harshitha</p>
  </footer>
</body>
</html>

administration.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Our Team - Harshitha Restaurant</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>Our Team</h1>
    <nav>
      <a href="index.html">Home</a>
      <a href="menu.html">Menu</a>
      <a href="about.html">About Us</a>
      <a href="contact.html">Contact Us</a>
    </nav>
  </header>
  <main>
    <section>
      <h2>Meet Our Team</h2>
      <div class="team">
        <div class="member">
          <img src="harshu.jpeg" alt="Harshitha - Manager">
          <p>Harshitha - Manager</p>
        </div>
        <div class="member">
          <img src="s1.jpeg" alt="Jane Smith - Chef">
          <p>Jane Smith - Chef</p>
        </div>
        <div class="member">
          <img src="s2.jpeg" alt="Sam Lee - Waiter">
          <p>Sam Lee - Waiter</p>
        </div>
      </div>
    </section>
  </main>
  <footer>
    <p>&copy; 2024 Harshitha</p>
  </footer>
</body>
</html>

contact.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Contact Us - Harshitha Restaurant</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>Contact Us</h1>
    <nav>
      <a href="index.html">Home</a>
      <a href="menu.html">Menu</a>
      <a href="about.html">About Us</a>
      <a href="administration.html">Our Team</a>
    </nav>
  </header>
  <main>
    <section>
      <h2>Get in Touch</h2>
      <img src="contact.jpeg" alt="Contact Banner" class="contact-banner">
      <p>Address: 123 Food Street, Chennai, India</p>
      <p>Phone: +91 9876543210</p>
      <p>Email: contact@restaurant.com</p>
    </section>
  </main>
  <footer>
    <p>&copy; 2024 Harshitha</p>
  </footer>
</body>
</html>

menu.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Menu</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>Our Menu</h1>
    <nav>
      <a href="index.html">About Me</a>
      <a href="menu.html">Menu</a>
      <a href="administration.html">Administration</a>
      <a href="contact.html">Contact Us</a>
    </nav>
  </header>
  <main>
    <img src="res.jpeg" alt="Menu Banner" class="menu-banner">
    <h2>Delicious Dishes</h2>
    <div class="menu-grid">
      <div class="menu-item" onclick="showDetails('cake', 'images/ca.jpg')">
        <img src="ca.jpeg" alt="cake">
        <p>cake</p>
      </div>
      <div class="menu-item" onclick="showDetails('cheese cake', 'images/d1.jpg')">
        <img src="d1.jpeg" alt="cheese cake">
        <p>cheese cake</p>
      </div>
      <div class="menu-item" onclick="showDetails('apple pie', 'images/d3.jpg')">
        <img src="d3.jpeg" alt="apple pie">
        <p>apple pie</p>
      </div>
      <div class="menu-item" onclick="showDetails('tiramisu', 'images/d4.jpg')">
        <img src="d4.jpeg" alt="tiramisu">
        <p>tiramisu</p>
      </div>
    </div>
    <div id="food-details" class="food-details">
      <!-- Food details will display dynamically here -->
    </div>
  </main>
  <footer>
    <p>&copy; 2024 Harshitha</p>
  </footer>
  <script>
    function showDetails(name, imgSrc) {
      const details = document.getElementById('food-details');
      details.innerHTML = `
        <h3>${name}</h3>
        <img src="${imgSrc}" alt="${name}" style="width:300px; height:auto; margin-top:10px;">
      `;
    }
  </script>
</body>
</html>

about.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Harshitha Restaurant</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>Harshitha Restaurant</h1>
    <nav>
      <a href="index.html">Home</a>
      <a href="menu.html">Menu</a>
      <a href="administration.html">Our Team</a>
      <a href="contact.html">Contact Us</a>
    </nav>
  </header>
  <main>
    <section>
      <h2>Welcome to Harshitha Restaurant</h2>
      <img src="about.jpeg" alt="Restaurant Image" class="about-image">
      <p>Located in the heart of Chennai, Harshitha Restaurant offers a memorable dining experience with a focus on high-quality food and exceptional service. Our mission is to provide a wide variety of delicious dishes made from fresh, locally sourced ingredients in a warm and inviting atmosphere.</p>
      <p>Whether it's a casual meal or a special occasion, we have something for everyone!</p>
    </section>
  </main>
  <footer>
    <p>&copy; 2024 Harshitha</p>
  </footer>
</body>
</html>

style.css
```
index.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Our Restaurant</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>Avanthika RESTAURANT</h1>
    <nav>
      <a href="about.html">About Us</a>
      <a href="menu.html">Menu</a>
      <a href="administration.html">Team</a>
      <a href="contact.html">Contact Us</a>
    </nav>
  </header>

  <section id="logo-details">
    <div class="logo-container">
      <img src="index.jpeg" alt="Restaurant Logo" class="restaurant-logo">
    </div>
    <div class="restaurant-details">
      <h2>Welcome to Avanthika Restaurant</h2>
      <p>Located in the heart of Chennai, Avanthika Restaurant offers a memorable dining experience with a focus on high-quality food and exceptional service. Our mission is to provide a wide variety of delicious dishes made from fresh, locally sourced ingredients in a warm and inviting atmosphere. Whether it's a casual meal or a special occasion, we have something for everyone!</p>
    </div>
  </section>

  <main>
    <section id="about">
        <h2>About Us</h2>
        <p>Learn more about our restaurant and the experience we offer to our customers. Click on the "About Us" link in the navigation to explore more.</p>
    </section>

  </main>

  <footer>
    <p>&copy; 2024 Avanthika</p>
  </footer>
</body>
</html>

administration.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Our Team - Avanthika Restaurant</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>Our Team</h1>
    <nav>
      <a href="index.html">Home</a>
      <a href="menu.html">Menu</a>
      <a href="about.html">About Us</a>
      <a href="contact.html">Contact Us</a>
    </nav>
  </header>
  <main>
    <section>
      <h2>Meet Our Team</h2>
      <div class="team">
        <div class="member">
          <img src="d1.jpeg" alt="Avanthika - Manager">
          <p>Avanthika - Manager</p>
        </div>
        <div class="member">
          <img src="d2.jpeg" alt="Jane Smith - Chef">
          <p>Jane Smith - Chef</p>
        </div>
        <div class="member">
          <img src="d3.jpeg" alt="Sam Lee - Waiter">
          <p>Sam Lee - Waiter</p>
        </div>
      </div>
    </section>
  </main>
  <footer>
    <p>&copy; 2024 Avanthika</p>
  </footer>
</body>
</html>

menu.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Menu</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>Our Menu</h1>
    <nav>
      <a href="index.html">About Me</a>
      <a href="menu.html">Menu</a>
      <a href="administration.html">Administration</a>
      <a href="contact.html">Contact Us</a>
    </nav>
  </header>
  <main>
    <img src="menu.jpeg" alt="Menu Banner" class="menu-banner">
    <h2>Delicious Dishes</h2>
    <div class="menu-grid">
      <div class="menu-item" onclick="showDetails('cake', 'images/ca.jpg')">
        <img src="cake.jpeg" alt="cake">
        <p>cake</p>
      </div>
      <div class="menu-item" onclick="showDetails('cheese cake', 'images/d1.jpg')">
        <img src="cheese cake.jpeg" alt="cheese cake">
        <p>cheese cake</p>
      </div>
      <div class="menu-item" onclick="showDetails('apple pie', 'images/d3.jpg')">
        <img src="apple pie.jpeg" alt="apple pie">
        <p>apple pie</p>
      </div>
      <div class="menu-item" onclick="showDetails('tiramisu', 'images/d4.jpg')">
        <img src="tiramasu.jpeg" alt="tiramisu">
        <p>tiramisu</p>
      </div>
    </div>
    <div id="food-details" class="food-details">
      <!-- Food details will display dynamically here -->
    </div>
  </main>
  <footer>
    <p>&copy; 2024 Avanthika</p>
  </footer>
  <script>
    function showDetails(name, imgSrc) {
      const details = document.getElementById('food-details');
      details.innerHTML = `
        <h3>${name}</h3>
        <img src="${imgSrc}" alt="${name}" style="width:300px; height:auto; margin-top:10px;">
      `;
    }
  </script>
</body>
</html>

contact.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Contact Us - Avanthika Restaurant</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>Contact Us</h1>
    <nav>
      <a href="index.html">Home</a>
      <a href="menu.html">Menu</a>
      <a href="about.html">About Us</a>
      <a href="administration.html">Our Team</a>
    </nav>
  </header>
  <main>
    <section>
      <h2>Get in Touch</h2>
      <img src="contact.jpeg" alt="Contact Banner" class="contact-banner">
      <p>Address: 123 Food Street, Chennai, India</p>
      <p>Phone: +91 9876543210</p>
      <p>Email: contact@restaurant.com</p>
    </section>
  </main>
  <footer>
    <p>&copy; 2024 Avanthika</p>
  </footer>
</body>
</html>

about.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Avanthika Restaurant</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>Avanthika Restaurant</h1>
    <nav>
      <a href="index.html">Home</a>
      <a href="menu.html">Menu</a>
      <a href="administration.html">Our Team</a>
      <a href="contact.html">Contact Us</a>
    </nav>
  </header>
  <main>
    <section>
      <h2>Welcome to Avanthika Restaurant</h2>
      <img src="about.jpeg" alt="Restaurant Image" class="about-image">
      <p>Located in the heart of Chennai, Avanthika Restaurant offers a memorable dining experience with a focus on high-quality food and exceptional service. Our mission is to provide a wide variety of delicious dishes made from fresh, locally sourced ingredients in a warm and inviting atmosphere.</p>
      <p>Whether it's a casual meal or a special occasion, we have something for everyone!</p>
    </section>
  </main>
  <footer>
    <p>&copy; 2024 Avanthika</p>
  </footer>
</body>
</html>
```


## OUTPUT:
![alt text](<avanthi/restapp/static/Screenshot (6).png>)
![alt text](<avanthi/restapp/static/Screenshot (7).png>)
![alt text](<avanthi/restapp/static/Screenshot (8).png>)
![alt text](<avanthi/restapp/static/Screenshot (9).png>)
## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
