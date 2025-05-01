# Ex.07 Restaurant Website
# Date:01/05/2025
# AIM:
To develop a static Restaurant website to display the food items and services provided by them.

# DESIGN STEPS:
## Step 1:
Requirement collection.

## Step 2:
Creating the layout using HTML and CSS.

## Step 3:
Updating the sample content.

## Step 4:
Choose the appropriate style and color scheme.

## Step 5:
Validate the layout in various browsers.

## Step 6:
Validate the HTML code.

## Step 7:
Publish the website in the given URL.

# PROGRAM:

'''
website.html

<!DOCTYPE html>
<html lang="en">
  
<head>
  
  <meta charset="UTF-8" />
  
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Sunday Splash | Restaurant</title>
  <style>
    * {
      
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Segoe UI', sans-serif;
    }

    body {
      line-height: 1.6;
      color: #333;
      background-color: #fdfdfd;
    }

    header {
      background: url('bg.png') no-repeat center center/cover;
      height: 100vh;
      color: white;
      text-align: center;
      display: flex;
      flex-direction: column;
      justify-content: center;
      padding: 0 20px;
    }

    header h1 {
      font-size: 4rem;
      margin-bottom: 10px;
    }

    header p {
      font-size: 1.5rem;
    }

    nav {
      background-color: #222;
      display: flex;
      justify-content: center;
      padding: 15px 0;
      position: sticky;
      top: 0;
      z-index: 100;
    }

    nav a {
      color: white;
      margin: 0 20px;
      text-decoration: none;
      font-weight: bold;
      transition: color 0.3s ease;
    }

    nav a:hover {
      color: #f4b400;
    }

    section {
      
      background: url('bgg.png') no-repeat center center/cover;
      height: 100vh;
      color:rgb(249, 243, 243);
      text-align: center;
      display: flex;
      flex-direction: column;
      justify-content: center;
      padding: 0 20px;
    }
    .menu {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }

    .menu-item {
      background:rgb(16, 16, 16);
      border: 1px solid #111111;
      border-radius: 10px;
      padding: 20px;
      text-align: center;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }

    .menu-item img {
      max-width: 100%;
      border-radius: 8px;
    }

    .chef-name {
      font-style: italic;
      font-size: 0.9rem;
      color: #121212;
      margin-top: 5px;
    }

    .chefs {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 40px;
      margin-top: 40px;
    }

    .chef-card {
      background: rgb(17, 17, 17);
      border: 1px solid #ddd;
      border-radius: 10px;
      text-align: center;
      padding: 20px;
      width: 250px;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }

    .chef-card img {

      width: 150px;
      height: 150px;
      object-fit: cover;
      border-radius: 50%;
      margin-bottom: 15px;
    }

    .about, .contact, .book {
      background-color: #f4f4f4;
      border-radius: 10px;
      padding: 30px;
    }

    .book form {
      display: flex;
      flex-direction: column;
      gap: 15px;
    }

    .book input, .book textarea {
      padding: 10px;
      border: 1px solid #fbf8f8;
      border-radius: 5px;
    }

    .book button {
      background-color: #222;
      color: rgb(253, 251, 251);
      padding: 10px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      font-weight: bold;
    }

    .book button:hover {
      background-color: #f4b400;
      color: #000;
    }

    footer {
      text-align: center;
      padding: 20px;
      background-color: #222;
      color: rgb(179, 173, 173);
    }

    @media (max-width: 600px) {
      header h1 {
        font-size: 2.5rem;
      }

      nav {
        flex-direction: column;
      }

      nav a {
        margin: 10px 0;
      }

      .chefs {
        flex-direction: column;
        align-items: center;
      }
    }
  </style>
</head>
<body>

  <header>
    <h1>SUNDAY SPLASH</h1>
    <p>Experience the taste of luxury</p>
  </header>

  <nav>
    
    <a href="#menu">Menu</a>
    <a href="#chefs">Chefs</a>
    <a href="#book">Book</a>
    <a href="#about">About</a>
    <a href="#contact">Contact</a>
  </nav>

  <section id="menu">
    <h2>Our Menu</h2>
    
    <div class="menu">
      <div class="menu-item">
        <img src="biryani.png" alt="Biryani">
        <h3>Biryani</h3>
        
      </div>
      <div class="menu-item">
        <img src="karidosa.png" alt="Karidosa">
        <h3>Karidosa</h3>
        
      </div>
      <div class="menu-item">
        <img src="shawarma.png" alt="Shawarma">
        <h3>Shawarma</h3>
        
      </div>
      <div class="menu-item">
        <img src="chocolava.png" alt="Chocolava Cake">
        <h3>Chocolava Cake</h3>
        
      </div>
      <div class="menu-item">
        <img src="soup.png" alt="Soup">
        <h3>Soup</h3>
        
      </div>
      <div class="menu-item">
        <img src="strawberry.png" alt="Chocolate Dipped Strawberry">
        <h3>Chocolate Dipped Strawberry</h3>
       
      </div>
      <div class="menu-item">
        <img src="tikka.png" alt="Chicken Tikka">
        <h3>Chicken Tikka</h3>
       
      </div>
      <div class="menu-item">
        <img src="pizza.png" alt="Pizza">
        <h3>Pizza</h3>
       
      </div>
      <div class="menu-item">
        <img src="icecream.png" alt="Icecream">
        <h3>Icecream</h3>
       
      </div>
      <div class="menu-item">
        <img src="cakes.png" alt="Rainbow Cake">
        <h3>Rainbow Cake</h3>
       
      </div>
    </div>
  </section>
  </section>

  
    <section id="chefs">
        <h2>Meet Our Chefs</h2>
        <div class="chefs">
          <div class="chef-card">
            <img src="bhatt.png" alt="Chef Venkatesh Bhatt">
            <h3>Chef Venkatesh Bhatt</h3>
            <p>Master of vegetarian food items and dessert items.One of the greatest chefs of India.</p>
          </div>
          <div class="chef-card">
            <img src="madhampatti.png" alt="Chef Madhampatti Ranganadhan">
            <h3>Chef Madhampatti Ranganadhan</h3>
            <p>Master in authentic and traditional non-vegetarian food items of Tamilnadu and India.</p>
          </div>
        </div>
      </section>
    
  </section>

  <section id="book" class="book">
    <h2>Book a Table</h2>
    <form>
      
      <input type="text" placeholder="Full Name" required>
      <input type="email" placeholder="Email Address" required>
      <input type="tel" placeholder="Phone Number" required>
      <input type="date" required>
      <input type="time" required>
      <input type="number" placeholder="Number of Guests" required>
      <textarea placeholder="Special Requests"></textarea>
      <button type="submit">Reserve Now</button>
    </form>
  </section>

  <section id="about" class="about">
    <h2>About Us</h2>
    <p>Sunday Splash is a fine dining restaurant in the heart of the city...First ever dining restaurant in the food town.</p>
  </section>

  <section id="contact" class="contact">
    <h2>Contact</h2>
    <p><strong>Address:</strong> Food Town,Hyderabad</p>
    <p><strong>Phone:</strong> 044-4858-4858</p>
    <p><strong>Email:</strong> sundaysplash@gmail.com</p>
  </section>

  <footer>
    <p>&copy; 2025 Sunday Splash. All rights reserved.</p>
  </footer>

</body>
</html>

'''




# OUTPUT:
![Screenshot 2025-05-01 143531](https://github.com/user-attachments/assets/b2191eee-8d50-40eb-99cf-67f1c8766445)
![Screenshot 2025-05-01 143624](https://github.com/user-attachments/assets/e853ef14-f578-424b-8c24-041d28586d11)
![Screenshot 2025-05-01 143651](https://github.com/user-attachments/assets/47d35807-4a11-43a8-abe6-62bb6f846d07)
![Screenshot 2025-05-01 143705](https://github.com/user-attachments/assets/301a6f1e-2333-4544-b5de-9d863483e7df)
![Screenshot 2025-05-01 143719](https://github.com/user-attachments/assets/a73a6166-328b-4110-817a-4034ba0e605b)
![Screenshot 2025-05-01 143732](https://github.com/user-attachments/assets/2c05dec5-836c-4bb5-8eca-76ef1afb6d55)



# RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
