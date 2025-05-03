# Ex.07 Restaurant Website
## Date: 03/05/25
## Name: Sanjit A , Register no: 212224220087

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
restaurant.html: 

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Courgette&family=Merienda:wght@300..900&display=swap" rel="stylesheet">
    <title>Foodie Restaurant</title>
    <style>
        body {
            margin: 0;
            font-family: 'Merienda', cursive;
            background: url('rest.jpg') no-repeat center center fixed;
            background-size: cover;
            color: rgb(255, 255, 255);
            display: flex;
            flex-direction: column;
            min-height: 100vh;
        }

        header {
            text-align: center;
            padding: 50px 20px;
            background: rgba(0, 0, 0, 0.5); 
            border-bottom: 2px solid goldenrod;
        }

        header h1 {
            font-size: 80px;
            letter-spacing: 10px;
            margin: 0;
            text-shadow: 2px 2px 8px black;
            animation: fadeIn 2s ease-in-out;
        }

        nav {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            background: rgba(0, 0, 0, 0.7); 
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.5);
            z-index: 1000;
        }

        nav ul {
            list-style: none;
            margin: 0;
            padding: 10px 20px;
            display: flex;
            justify-content: center;
            animation: slideDown 1.5s ease-out;
        }

        nav li {
            margin: 0 20px;
        }

        nav a {
            text-decoration: none;
            color: white;
            font-size: 18px;
            font-weight: 600;
            padding: 10px 20px;
            transition: all 0.3s ease-in-out;
            border-radius: 5px;
        }

        nav a:hover {
            color: black;
            background: linear-gradient(to right, goldenrod, gold);
            transform: scale(1.1);
        }

        main {
            flex: 1;
            padding: 40px;
            text-align: center;
            background: rgba(255, 255, 255, 0.1); 
            margin: 20px auto;
            max-width: 900px;
            border-radius: 15px;
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.7);
            animation: fadeInUp 1.5s ease-in-out;
        }

        main p {
            font-size: 24px;
            font-weight: 400;
            line-height: 1.5;
            color: #f9f9f9;
            text-shadow: 1px 1px 3px black;
        }

        footer {
            background: rgba(0, 0, 0, 0.8);
            color: white;
            text-align: center;
            padding: 20px 0;
            border-top: 2px solid goldenrod;
            box-shadow: 0 -4px 6px rgba(0, 0, 0, 0.5);
        }

        footer p {
            margin: 5px 0;
            font-size: 16px;
        }

        footer a {
            color: goldenrod;
            text-decoration: none;
            margin: 0 10px;
            font-size: 18px;
            transition: color 0.3s ease-in-out;
        }

        footer a:hover {
            color: #d4af37;
        }

        @media (max-width: 768px) {
            header h1 {
                font-size: 50px;
                letter-spacing: 5px;
            }

            nav a {
                font-size: 16px;
                padding: 8px 12px;
            }

            main p {
                font-size: 20px;
            }

            footer p, footer a {
                font-size: 16px;
            }
        }

        @keyframes fadeIn {
            from {
                opacity: 0;
            }
            to {
                opacity: 1;
            }
        }

        @keyframes slideDown {
            from {
                transform: translateY(-100%);
                opacity: 0;
            }
            to {
                transform: translateY(0);
                opacity: 1;
            }
        }

        @keyframes fadeInUp {
            from {
                transform: translateY(20px);
                opacity: 0;
            }
            to {
                transform: translateY(0);
                opacity: 1;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Foodie Restaurant</h1>
    </header>
    <nav>
        <ul>
            <li><a href="#" title="Home">Home</a></li>
            <li><a href="menu.html" title="Menu">Menu</a></li>
            <li><a href="administration.html" title="Administration">Administration</a></li>
            <li><a href="contact.html" title="Contact Us">Contact Us</a></li>
        </ul>
    </nav>
    <main>
        <p>Welcome to Foodie Restaurant! Indulge in a delightful dining experience, where taste meets perfection. Explore our menu and immerse yourself in a world of exquisite flavors.</p>
    </main>
    <footer>
        <p>&copy; 2025 Foodie Restaurant | Designed by: <b>Sanjit A</b></p>
        <p>
            <a href="#" title="Facebook">Facebook</a> |
            <a href="#" title="Twitter">Twitter</a> |
            <a href="#" title="Instagram">Instagram</a>
        </p>
    </footer>
</body>
</html>
```

```
menu.html:

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Restaurant Menu</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(135deg, #f0f0f0, #e0e0e0);
            color: #333;
        }
        header {
            background-color: #8b0000;
            color: white;
            padding: 20px 0;
            text-align: center;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
        }
        header h1 {
            margin: 0;
            font-size: 3rem;
        }
        header p {
            font-size: 1.2rem;
            margin-top: 5px;
            font-weight: lighter;
        }
        .menu-section {
            max-width: 1200px;
            margin: 40px auto;
            padding: 0 20px;
        }
        .menu-section h2 {
            text-align: center;
            margin-bottom: 20px;
            font-size: 2.5rem;
            color: #8b0000;
            border-bottom: 3px solid #ddd;
            display: inline-block;
            padding-bottom: 5px;
        }
        .menu-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        .menu-item {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            text-align: center;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .menu-item:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.15);
        }
        .menu-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }
        .menu-item h3 {
            margin: 15px 0 10px;
            font-size: 1.6rem;
            color: #333;
        }
        .menu-item p {
            color: #555;
            font-size: 1rem;
            margin: 0 10px 15px;
        }
        .menu-item .price {
            font-weight: bold;
            font-size: 1.2rem;
            color: #8b0000;
            margin-bottom: 15px;
        }
        footer {
            text-align: center;
            padding: 15px 0;
            background-color: #333;
            color: white;
            margin-top: 40px;
        }
    </style>
</head>
<body>

<header>
    <h1>Delicious Indian Bites</h1>
    <p>Your favorite spot for authentic Indian non-veg meals</p>
</header>

<div class="menu-section">
    <h2>Biriyani</h2>
    <div class="menu-grid">
        <div class="menu-item">
            <img src="chicken.jpg" alt="Chicken Biriyani">
            <h3>Chicken Biriyani</h3>
            <p>Fragrant rice cooked with chicken, spices, and herbs.</p>
            <div class="price">₹350</div>
        </div>
        <div class="menu-item">
            <img src="mutton.jpg" alt="Mutton Biriyani">
            <h3>Mutton Biriyani</h3>
            <p>Slow-cooked mutton with aromatic basmati rice.</p>
            <div class="price">₹450</div>
        </div>
        <div class="menu-item">
            <img src="prawn.jpg" alt="Prawn Biriyani">
            <h3>Prawn Biriyani</h3>
            <p>Succulent prawns cooked with flavorful biriyani rice.</p>
            <div class="price">₹500</div>
        </div>
        <div class="menu-item">
            <img src="egg.jpg" alt="Egg Biriyani">
            <h3>Egg Biriyani</h3>
            <p>Soft-boiled eggs mixed with rich biriyani rice.</p>
            <div class="price">₹300</div>
        </div>
        <div class="menu-item">
            <img src="khuska.jpeg" alt="Khuska">
            <h3>Khuska</h3>
            <p>A simple, aromatic rice dish cooked with spices.</p>
            <div class="price">₹250</div>
        </div>
    </div>
</div>

<div class="menu-section">
    <h2>Starters</h2>
    <div class="menu-grid">
        <div class="menu-item">
            <img src="crispy.webp" alt="Crispy Golden Chicken">
            <h3>Crispy Golden Chicken</h3>
            <p>Deep-fried, golden chicken wings with a crispy coating.</p>
            <div class="price">₹180</div>
        </div>
        <div class="menu-item">
            <img src="mutton95.jpg" alt="Mutton 95">
            <h3>Mutton 95</h3>
            <p>Spicy and crispy mutton chunks with a flavorful sauce.</p>
            <div class="price">₹220</div>
        </div>
        <div class="menu-item">
            <img src="fish.jpg" alt="Fish Fry">
            <h3>Fish Fry</h3>
            <p>Fresh fish marinated and fried to perfection.</p>
            <div class="price">₹250</div>
        </div>
        <div class="menu-item">
            <img src="prawnfry.jpg" alt="Crispy Prawn Fry">
            <h3>Crispy Prawn Fry</h3>
            <p>Delicious prawns deep-fried with a crispy, spicy coating.</p>
            <div class="price">₹280</div>
        </div>
    </div>
</div>

<div class="menu-section">
    <h2>Tandoori and Kebab</h2>
    <div class="menu-grid">
        <div class="menu-item">
            <img src="kebab.webp" alt="Chicken Kebab">
            <h3>Chicken Kebab</h3>
            <p>Grilled chicken marinated in flavorful spices.</p>
            <div class="price">₹220</div>
        </div>
        <div class="menu-item">
            <img src="Tandoori.jpg" alt="Tandoori Chicken">
            <h3>Tandoori Chicken</h3>
            <p>Smoky tandoori chicken.</p>
            <div class="price">₹450</div>
        </div>
        <div class="menu-item">
            <img src="reshmi.jpg" alt="Reshmi Chicken Kebab">
            <h3>Reshmi Chicken  Kebab</h3>
            <p>Soft and juicy chicken kebabs with creamy marinade.</p>
            <div class="price">₹250</div>
        </div>
        <div class="menu-item">
            <img src="garlic.jpg" alt="Garlic Chicken">
            <h3>Garlic Chicken</h3>
            <p>Delicious chicken kebabs flavored with garlic and spices.</p>
            <div class="price">₹270</div>
        </div>
    </div>
</div>

<div class="menu-section">
    <h2>Gravies</h2>
    <div class="menu-grid">
        <div class="menu-item">
            <img src="butter.webp" alt="Butter Chicken Masala">
            <h3>Butter Chicken Masala</h3>
            <p>Creamy chicken gravy with a rich tomato base.</p>
            <div class="price">₹350</div>
        </div>
        <div class="menu-item">
            <img src="mgravy.jpg" alt="Spicy Mutton Gravy">
            <h3>Spicy Mutton Gravy</h3>
            <p>Rich and spicy mutton gravy made with aromatic spices.</p>
            <div class="price">₹450</div>
        </div>
        <div class="menu-item">
            <img src="prawng.jpg" alt="Prawn Gravy">
            <h3>Prawn Gravy</h3>
            <p>Fresh prawns cooked in a spicy, tangy gravy.</p>
            <div class="price">₹500</div>
        </div>
        <div class="menu-item">
            <img src="cheti.jpg" alt="Chettinad Pepper Chicken Gravy">
            <h3>Chettinad Pepper Chicken Gravy</h3>
            <p>Chicken cooked in a spicy and flavorful Chettinad gravy.</p>
            <div class="price">₹380</div>
        </div>
    </div>
</div>

<div class="menu-section">
    <h2>Breads</h2>
    <div class="menu-grid">
        <div class="menu-item">
            <img src="chap.jpg" alt="Chapatti">
            <h3>Chapatti</h3>
            <p>Soft whole wheat flatbread.</p>
            <div class="price">₹40</div>
        </div>
        <div class="menu-item">
            <img src="butn.jpg" alt="Butter Naan">
            <h3>Butter Naan</h3>
            <p>Soft, pillowy leavened bread.</p>
            <div class="price">₹60</div>
        </div>
        <div class="menu-item">
            <img src="par.webp" alt="Parotta">
            <h3>Parotta</h3>
            <p>Flaky and soft South Indian flatbread.</p>
            <div class="price">₹60</div>
        </div>
        <div class="menu-item">
            <img src="kot.jpg" alt="Kothu Parotta">
            <h3>Kothu Parotta</h3>
            <p>Shredded parotta mixed with meat and spices.</p>
            <div class="price">₹120</div>
        </div>
    </div>
</div>

<div class="menu-section">
    <h2>Deserts</h2>
    <div class="menu-grid">
        <div class="menu-item">
            <img src="gula.webp" alt="Gulab Jamun">
            <h3>Gulab Jamun</h3>
            <p>Sweet, syrup-soaked deep-fried dough balls.</p>
            <div class="price">₹100</div>
        </div>
        <div class="menu-item">
            <img src="ras.jpg" alt="Rasamalai">
            <h3>Rasamalai</h3>
            <p>Soft cheese dumplings soaked in sweet milk.</p>
            <div class="price">₹180</div>
        </div>
        <div class="menu-item">
            <img src="rose.jpg" alt="Rose Milk">
            <h3>Rose Milk</h3>
            <p>Chilled rose-flavored milk served with ice.</p>
            <div class="price">₹60</div>
        </div>
        <div class="menu-item">
            <img src="bad.jpeg" alt="Badham Milk">
            <h3>Badham Milk</h3>
            <p>Chilled almond milk with crushed nuts.</p>
            <div class="price">₹70</div>
        </div>
    </div>
</div>

<footer>
    <p>&copy; 2025 Delicious Indian Bites. All rights reserved.</p>
</footer>

</body>
</html>
```

```
administration.html:

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chefs</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Caveat:wght@700&family=Pacifico&display=swap" rel="stylesheet">
    <style>
        body {
            margin: 0;
            padding: 0;
            font-family: Arial, sans-serif;
            background-color: #f8f8f8;
        }

        
        header {
            text-align: center;
            background-color: #b5651d;
            padding: 20px 0;
        }

        header h1 {
            font-family: "Caveat", cursive;
            font-size: 50px;
            color: white;
            margin: 0;
        }

       
        .chefs-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            padding: 40px;
            max-width: 1200px;
            margin: auto;
        }

        .chef-card {
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            text-align: center;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .chef-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
        }

        .chef-card img {
            width: 100%;
            object-fit: contain; 
            max-height: 300px; 
        }

        .chef-details {
            padding: 20px;
        }

        .chef-details h1 {
            font-size: 20px;
            color: #b5651d;
            margin: 10px 0;
        }

        .chef-details h2,
        .chef-details h3 {
            font-size: 16px;
            color: #555;
            margin: 5px 0;
        }

        
        footer {
            text-align: center;
            background-color: #333;
            color: white;
            padding: 10px 0;
            margin-top: 40px;
        }

        footer p {
            margin: 0;
        }
    </style>
</head>
<body>

    
    <header>
        <h1>Our Chefs</h1>
    </header>

   
    <div class="chefs-container">
        <div class="chef-card">
            <img src="c1.png" alt="Gal Gadot">
            <div class="chef-details">
                <h1>Miss Gal Gadot</h1>
                <h2>Designation: Sous Chef</h2>
                <h3>Experience: 3 years</h3>
            </div>
        </div>
        <div class="chef-card">
            <img src="c2.png" alt="Ryan">
            <div class="chef-details">
                <h1>Mr. Ryan</h1>
                <h2>Designation: Executive Chef</h2>
                <h3>Experience: 7 years</h3>
            </div>
        </div>
        <div class="chef-card">
            <img src="c3.png" alt="Chef Vijay Joseph">
            <div class="chef-details">
                <h1>Mr. Vijay Joseph</h1>
                <h2>Designation: Saucier Chef</h2>
                <h3>Experience: 2 years</h3>
            </div>
        </div>
        <div class="chef-card">
            <img src="c4.png" alt="Chef Hemsworth">
            <div class="chef-details">
                <h1>Mr. Hemsworth</h1>
                <h2>Designation: Pastry Chef</h2>
                <h3>Experience: 3 years</h3>
            </div>
        </div>
        <div class="chef-card">
            <img src="c5.jpg" alt="Chef Sharukh">
            <div class="chef-details">
                <h1>Mr. Sharukh</h1>
                <h2>Designation: Pantry Chef</h2>
                <h3>Experience: 4 years</h3>
            </div>
        </div>
        <div class="chef-card">
            <img src="c6.jpg" alt="Chef Sudharsin">
            <div class="chef-details">
                <h1>Mr. Sudarsin</h1>
                <h2>Designation: Butcher Chef</h2>
                <h3>Experience: 6 months</h3>
            </div>
        </div>
    </div>

    
    <footer>
        <p>&copy; 2025 Foodie's Paradise. All rights reserved.</p>
    </footer>

</body>
</html>
```

```
contact.html:

<html>
    <head>
        <link rel="preconnect" href="https://fonts.googleapis.com">
        <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
        <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@400..700&display=swap" rel="stylesheet">
        <title>Contact Us</title>
        <style>
            #n1{
                position: relative;
                color: red;
                font-size: 60px;
                padding-left: 380px;
                left: 0px;
                top: 190px;
                letter-spacing: 5px;
            }
            body{
                background-image: url(last.jpg);
                background-repeat: no-repeat;
                background-size: 1700px 950px;
            }
            #n2{
                position:relative;
                color: black;
                font-size: 80px;
                padding-left: 480px;
                top: 140px;
                letter-spacing: 3px;
                font-family: "Dancing Script", cursive;
            }
            #n3{
                position: relative;
                color: aliceblue;
                font-size: 35px;
                top: 255px;
                padding-left: 240px;
            }
            #n4{
                position: relative;
                color: red;
                font-size:31px;
                top: 205px;
                padding-left: 170px;
                letter-spacing: 2px;
            }
            #n5{
                position: relative;
                color: aliceblue;
                font-size: 35px;
                top: 60px;
                padding-left: 680px;
            }
            #n6{
                position: relative;
                color: red;
                font-size:35px;
                top: 8px;
                padding-left: 505px;
            }
            #n7{
                position: relative;
                color: aliceblue;
                font-size: 35px;
                bottom: 135px;
                padding-left: 1155px;
            }
            #n8{
                position: relative;
                color: red;
                font-size: 31px;
                bottom: 187px;
                padding-left: 950px;
                text-align: center;
            }

            
            a {
                color: red;
                text-decoration: none;
                cursor: pointer;
            }

            
            a:hover {
                text-decoration: underline;
            }
            
        </style>
    </head>
    <body>
        <h1 id="n1">PERFECTLY BALANCED</h1>
        <h2 id="n2">Quality and Taste</h2>
        <h5 id="n3">Phone:</h5>
        <h5 id="n4">
            <a href="tel:+914415443595">+91 4415443595</a>
        </h5>
        <h5 id="n5">Email:</h5>
        <h5 id="n6">
            <a href="mailto:foodierestaurant@foodie.com"><b>foodierestaurant@foodie.com</b></a>
        </h5>
        <h5 id="n7">Location:</h5>
        <h5 id="n8">
            <a href="https://www.google.com/maps?q=1,+Foodie+restaurant+OMR+street+Perungudi"><b>1, Foodie restaurant OMR street Perungudi</b></a>
        </h5>
    </body>
</html>
```


## OUTPUT:
![alt text](<Screenshot 2025-05-03 122445.png>)

![alt text](<Screenshot 2025-05-03 122519.png>)

![alt text](<Screenshot 2025-05-03 122536.png>)

![alt text](<Screenshot 2025-05-03 122549.png>)

![alt text](<Screenshot 2025-05-03 122607.png>)

![alt text](<Screenshot 2025-05-03 122624.png>)

![alt text](<Screenshot 2025-05-03 122635.png>)

![alt text](<Screenshot 2025-05-03 122646.png>)

![alt text](<Screenshot 2025-05-03 122702.png>)

![alt text](<Screenshot 2025-05-03 122716.png>)

![alt text](<Screenshot 2025-05-03 122733.png>)


## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
