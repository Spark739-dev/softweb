# Ex.07 Restuarant Website
## Date:
23-10-2025
## AIM:
To develop a static Resturant website to display the menu and services provided by the resturant.

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
## FOR LOOKPAGE(restdesign.html):
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>HIMALAYA BLISS - RESTAURANT DESIGN</title>
        <style>
            body {
                margin: 0;
                font-family: 'Courier New', monospace;
                background-color: #f1f3f1;
            }

        
            .header {
                text-align: center;
                padding: 30px 0;
            }

            .header img {
                height: 100px;
            }

            .header h1 {
                font-size: 2.5em;
                color: #3f5a52;
                letter-spacing: 3px;
                margin-top: 10px;
            }

            
            nav {
                display: flex;
                justify-content: center;
                background-color: #2f2f2f;
                border-radius: 20px;
                width: 90%;
                max-width: 1200px;
                margin: 0 auto 30px auto; 
            }

            nav a {
                color: white;
                text-decoration: none;
                font-weight: bold;
                padding: 20px 40px;
                font-size: 1.2em;
                transition: background 0.3s;
            }

            nav a:hover {
                background-color: #3f5a52;
                border-radius: 20px;
            }

            
            .main-hero-image {
                display: block; 
                max-width: 90%;
                height: auto;
                margin: 30px auto;
                border-radius: 15px;
                box-shadow: 0 8px 16px rgba(0,0,0,0.3);
            }

            .image-gallery {
                display: flex;
                flex-wrap: wrap;
                justify-content: center;
                gap: 20px;
                padding: 20px;
                max-width: 1200px;
                margin: 0 auto;
            }

            .image-gallery img {
                max-width: 100%;
                height: auto;
                width: 300px;
                border-radius: 10px;
                box-shadow: 0 4px 8px rgba(0,0,0,0.2);
            }

            @media (max-width: 768px) {
                nav a {
                    padding: 15px 15px;
                    font-size: 1em;
                }
            }
        </style>
    </head>
    <body>

        <div class="header">
            <img src="header.png" alt="HIMALAYA BLISS LOGO">
            <h1>HIMALAYA BLISS</h1>
        </div>

        <nav>
            <a href="home.html">Home</a>
            <a href="menus1.html">Menu</a>
            <a href="admins1.html">Administration</a>
            <a href="contact.html">Contact Us</a>
        </nav>
        
        

        <div class="image-gallery">
            <img src="images1.jpeg" alt="FOODS1">
            <img src="images2.webp" alt="FOODS2">
            <img src="images3.jpeg" alt="FOODS3">
        </div>

    </body>
    </html>

## FOR HOMEPAGE(home.html):
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Restaurant Home Section</title>
        <style>
            
            body {
                font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
                margin: 0;
                padding: 20px; 
                background-color: #f0f0f0; 
                display: flex;
                justify-content: center;
                align-items: flex-start; 
                min-height: 100vh;
                box-sizing: border-box;
            }

            
            .home-section-container {
                width: 100%;
                max-width: 1200px; 
                display: flex;
                flex-wrap: wrap; 
                gap: 30px; 
                justify-content: center; 
                padding: 30px 0;
            }

            
            .info-card {
                background-color: #ffe0b2;  
                border-radius: 8px;
                box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
                overflow: hidden;
                flex: 1;  
                min-width: 280px;  
                max-width: 350px;  
                display: flex;
                flex-direction: column;
                color: #333;
                text-align: center;  
            }

            .card-title {
                font-size: 1.8em;
                font-weight: bold;
                color: #333;
                margin: 25px 20px 15px 20px;
            }

            .card-image {
                width: 100%;
                height: 200px; 
                overflow: hidden;
                display: flex;
                justify-content: center;
                align-items: center;
                margin-bottom: 20px;
            }

            .card-image img {
                width: 100%;
                height: 100%;
                object-fit: cover;  
                display: block;
            }

            .card-content {
                padding: 0 20px 25px 20px;  
                flex-grow: 1;  
                display: flex;
                flex-direction: column;
            }

            .card-content p {
                font-size: 0.95em;
                line-height: 1.6;
                color: #555;
                margin-bottom: 20px;
            }

            .card-link {
                display: inline-block;
                color: #007bff;  
                text-decoration: none;
                font-weight: 600;
                margin-top: auto;  
            }

            .card-link:hover {
                text-decoration: underline;
            }

            
            .booking-form {
                text-align: left;  
            }

            .form-group {
                margin-bottom: 15px;
            }

            .form-group label {
                display: block;
                margin-bottom: 5px;
                font-size: 0.9em;
                color: #444;
                font-weight: 600;
            }

            .form-group input[type="date"],
            .form-group input[type="time"],
            .form-group input[type="number"],
            .form-group input[type="text"] {  
                width: calc(100% - 20px);  
                padding: 10px;
                border: 1px solid #ccc;
                border-radius: 4px;
                font-size: 0.9em;
                box-sizing: border-box;
            }
            
            .form-group input[type="submit"] {
                background-color: #ff9800;  
                color: white;
                border: none;
                padding: 12px 20px;
                border-radius: 5px;
                font-size: 1em;
                cursor: pointer;
                transition: background-color 0.3s ease;
                width: 100%;
                margin-top: 10px;
            }

            .form-group input[type="submit"]:hover {
                background-color: #e68900;
            }

            
            .opening-hours-list {
                list-style: none;
                padding: 0;
                margin: 0;
                text-align: center; 
            }

            .opening-hours-list li {
                font-size: 1em;
                margin-bottom: 8px;
                color: #555;
            }
            .opening-hours-list li strong {
                color: #333;
            }


            
            @media (max-width: 992px) {
                .info-card {
                    max-width: 45%; 
                }
            }

            @media (max-width: 768px) {
                .home-section-container {
                    flex-direction: column; 
                    align-items: center;
                    padding: 20px 0;
                }
                .info-card {
                    min-width: unset;
                    width: 90%; 
                    max-width: 400px; 
                }
            }
        </style>
    </head>
    <body>

        <div class="home-section-container">

            <div class="info-card">
                <h2 class="card-title">Our New Menu</h2>
                <div class="card-image">
                    <img src="food1.jpg" alt="Variety of Asian dishes"> </div>
                <div class="card-content">
                    <p>Explore our latest culinary creations! Our chefs have curated a selection of dishes using the freshest seasonal ingredients, promising a delightful dining experience for every palate.</p>
                    <a href="menus1.html" class="card-link">See our menu</a>
                </div>
            </div>

            <div class="info-card">
                <h2 class="card-title">Book a Table</h2>
                <div class="card-image">
                    <img src="food2.jpg" alt="Variety of Indian dishes"> </div>
                <div class="card-content booking-form">
                    <p>Reserve your spot for an unforgettable dining experience. Fill out the form below and we'll confirm your booking shortly.</p>
                    <form action="#" method="POST">
                        <div class="form-group">
                            <label for="booking-name">Your Name:</label>
                            <input type="text" id="booking-name" name="name" required>
                        </div>
                        <div class="form-group">
                            <label for="booking-date">Date:</label>
                            <input type="date" id="booking-date" name="date" required>
                        </div>
                        <div class="form-group">
                            <label for="booking-time">Time:</label>
                            <input type="time" id="booking-time" name="time" required>
                        </div>
                        <div class="form-group">
                            <label for="booking-guests">Number of Guests:</label>
                            <input type="number" id="booking-guests" name="guests" min="1" max="10" value="2" required>
                        </div>
                        <div class="form-group">
                            <input type="submit" value="Book your table now">
                        </div>
                    </form>
                </div>
            </div>

            <div class="info-card">
                <h2 class="card-title">Opening Hours</h2>
                <div class="card-image">
                    <img src="food3.jpg" alt="Assortment of fresh food items"> </div>
                <div class="card-content">
                    <p>Plan your visit to our restaurant. We look forward to serving you our finest dishes during these hours:</p>
                    <ul class="opening-hours-list">
                        <li><strong>Mon - Fri:</strong> 2pm - 10pm</li>
                        <li><strong>Sat:</strong> 2pm - 11pm</li>
                        <li><strong>Sun:</strong> 2pm - 9pm</li>
                    </ul>
                    </div>
            </div>

        </div>

    </body>
    </html>

## FOR MENUPAGE(menus1.html):
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Restaurant Food Menu</title>
        <style>
            
            body {
                margin: 0;
                font-family: 'Georgia', serif;  
                background-color: #2c3e50; 
                display: flex;
                justify-content: center;
                align-items: center;
                min-height: 100vh;
                padding: 20px;
                box-sizing: border-box;
            }

            .menu-container {
                width: 100%;
                max-width: 900px;  
                background-color: #3f513f;  
                color: #f0f0f0;  
                border-radius: 10px;
                overflow: hidden;  
                box-shadow: 0 15px 40px rgba(0, 0, 0, 0.5);
                position: relative;
            }

            
            .menu-background {
                background-image: url('https://i.imgur.com/your_image_link_here.jpg');  
                background-size: cover;
                background-position: center;
                padding: 50px 70px;  
                position: relative;
                z-index: 1;
            }

            .menu-background::before {
                content: '';
                position: absolute;
                top: 0;
                left: 0;
                right: 0;
                bottom: 0;
                background-color: rgba(0, 0, 0, 0.2);  
                z-index: -1;
            }

            
            .menu-header {
                text-align: center;
                margin-bottom: 40px;
                position: relative;  
            }

            .menu-header .logo {
                position: absolute;
                top: 0px;  
                right: 0px;  
                width: 100px;  
                height: auto;
                color: #d4a762;  
                font-family: 'Times New Roman', serif;
                font-size: 0.8em;
                line-height: 1.2;
                text-align: right;
                padding: 10px;
                box-sizing: border-box;
            }
            .menu-header .logo strong {
                display: block;
                font-size: 1.2em;
                letter-spacing: 1px;
            }
            .menu-header .logo span {
                font-size: 0.8em;
                opacity: 0.8;
            }


            .menu-header h1 {
                font-family: 'Dancing Script', cursive;  
                font-size: 5em;
                color: #fff;  
                margin: 0;
                font-weight: normal;
            }

            
            .menu-content {
                display: flex;
                flex-wrap: wrap;  
                gap: 40px;  
                justify-content: space-between;
            }

            .menu-column {
                flex: 1;  
                min-width: 300px;  
                max-width: 48%;  
                box-sizing: border-box;
            }

            
            .menu-category {
                margin-bottom: 30px;
            }

            .menu-category h2 {
                font-family: 'Playfair Display', serif;  
                font-size: 1.8em;
                color: #d4a762;  
                text-transform: uppercase;
                letter-spacing: 2px;
                margin-bottom: 20px;
                padding-bottom: 5px;
                border-bottom: 1px solid rgba(212, 167, 98, 0.4);  
            }

            
            .menu-item {
                margin-bottom: 20px;
            }

            .item-title-price {
                display: flex;
                justify-content: space-between;
                align-items: flex-end;  
                margin-bottom: 5px;
            }

            .item-title {
                font-family: 'Lato', sans-serif;  
                font-size: 1.3em;
                color: #ffffff;  
                font-weight: 600;
            }

            .item-price {
                font-family: 'Lato', sans-serif;
                font-size: 1.3em;
                color: #d4a762;  
                font-weight: 600;
                margin-left: 15px;  
                white-space: nowrap;  
            }

            .item-description {
                font-family: 'Open Sans', sans-serif;  
                font-size: 0.95em;
                color: #e0e0e0;  
                line-height: 1.4;
                margin-top: -5px;  
            }

            
            .menu-footer {
                text-align: center;
                margin-top: 50px;
                color: #d4a762;
                font-family: 'Lato', sans-serif;
                font-size: 1.1em;
                letter-spacing: 1px;
            }

            
            @media (max-width: 768px) {
                .menu-background {
                    padding: 30px 40px;
                }
                .menu-header h1 {
                    font-size: 4em;
                }
                .menu-content {
                    flex-direction: column;  
                    gap: 20px;
                }
                .menu-column {
                    min-width: 100%;
                    max-width: 100%;
                }
                .menu-header .logo {
                    position: static;
                    text-align: center;
                    margin-bottom: 20px;
                }
            }
            @media (max-width: 480px) {
                .menu-background {
                    padding: 20px;
                }
                .menu-header h1 {
                    font-size: 3em;
                }
                .menu-category h2 {
                    font-size: 1.5em;
                }
                .item-title, .item-price {
                    font-size: 1.1em;
                }
                .item-description {
                    font-size: 0.9em;
                }
            }

            
            @import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@400;700&family=Playfair+Display:wght@400;700&family=Lato:wght@400;600&family=Open+Sans:wght@400&display=swap');
        </style>
    </head>
    <body>
        <div class="menu-container">
            <div class="menu-background">
                <div class="menu-header">
                    <div class="logo">
                        <strong>HIMALAYABLISS</strong><br>
                        <span>Restaurant of Heaven</span>
                    </div>
                    <h1>Menu</h1>
                </div>

                <div class="menu-content">
                    <div class="menu-column">
                        <div class="menu-category">
                            <h2>Appetizers</h2>
                            <div class="menu-item">
                                <div class="item-title-price">
                                    <span class="item-title">Caprese Skewers</span>
                                    <span class="item-price">$15.00</span>
                                </div>
                                <p class="item-description">Fresh mozzarella, cherry tomatoes, and basil, drizzled with balsamic glaze.</p>
                            </div>
                            <div class="menu-item">
                                <div class="item-title-price">
                                    <span class="item-title">Spicy Chicken Wings</span>
                                    <span class="item-price">$20.00</span>
                                </div>
                                <p class="item-description">Crispy wings tossed in a fiery house-made sauce, served with blue cheese dip.</p>
                            </div>
                            <div class="menu-item">
                                <div class="item-title-price">
                                    <span class="item-title">Vegetable Samosa</span>
                                    <span class="item-price">$10.00</span>
                                </div>
                                <p class="item-description">Savory pastry filled with spiced potatoes and peas, served with mint chutney.</p>
                            </div>
                            <div class="menu-item">
                                <div class="item-title-price">
                                    <span class="item-title">MUTTON 65</span>
                                    <span class="item-price">$4.00</span>
                                </div>
                                <p class="item-description">Spicy, deep-fried boneless mutton pieces, a Southern Indian delicacy.</p>
                            </div>
                            <div class="menu-item">
                                <div class="item-title-price">
                                    <span class="item-title">Tomato Soup</span>
                                    <span class="item-price">$10.00</span>
                                </div>
                                <p class="item-description">Creamy roasted tomato soup, served with herbed croutons.</p>
                            </div>
                        </div>

                        <div class="menu-category">
                            <h2>Salads</h2>
                            <div class="menu-item">
                                <div class="item-title-price">
                                    <span class="item-title">Quinoa Salad</span>
                                    <span class="item-price">$10.00</span>
                                </div>
                                <p class="item-description">Healthy quinoa with mixed greens, cranberries, and a citrus vinaigrette.</p>
                            </div>
                            <div class="menu-item">
                                <div class="item-title-price">
                                    <span class="item-title">Spinach Salad</span>
                                    <span class="item-price">$20.00</span>
                                </div>
                                <p class="item-description">Fresh spinach, strawberries, candied pecans, and poppy seed dressing.</p>
                            </div>
                            <div class="menu-item">
                                <div class="item-title-price">
                                    <span class="item-title">Eggplant Salad</span>
                                    <span class="item-price">$30.00</span>
                                </div>
                                <p class="item-description">Grilled eggplant, roasted bell peppers, and feta cheese with a lemon-herb dressing.</p>
                            </div>
                            <div class="menu-item">
                                <div class="item-title-price">
                                    <span class="item-title">Chicken Salad</span>
                                    <span class="item-price">$50.00</span>
                                </div>
                                <p class="item-description">Grilled chicken, crisp lettuce, tomatoes, and cucumber with a creamy dressing.</p>
                            </div>
                            <div class="menu-item">
                                <div class="item-title-price">
                                    <span class="item-title">Green Salad</span>
                                    <span class="item-price">$40.00</span>
                                </div>
                                <p class="item-description">Mixed seasonal greens with a light vinaigrette.</p>
                            </div>
                            <div class="menu-item">
                                <div class="item-title-price">
                                    <span class="item-title">Pasta Salad</span>
                                    <span class="item-price">$60.00</span>
                                </div>
                                <p class="item-description">Tricolor pasta, fresh vegetables, and Italian dressing.</p>
                            </div>
                        </div>
                    </div>

                    <div class="menu-column">
                        <div class="menu-category">
                            <h2>Main Courses</h2>
                            <div class="menu-item">
                                <div class="item-title-price">
                                    <span class="item-title">Beef Stir-Fry</span>
                                    <span class="item-price">$20.00</span>
                                </div>
                                <p class="item-description">Tender beef strips, crisp vegetables, and savory stir-fry sauce, served with rice.</p>
                            </div>
                            <div class="menu-item">
                                <div class="item-title-price">
                                    <span class="item-title">Shrimp Tacos</span>
                                    <span class="item-price">$10.00</span>
                                </div>
                                <p class="item-description">Grilled shrimp, fresh slaw, and spicy crema in soft tortillas.</p>
                            </div>
                            <div class="menu-item">
                                <div class="item-title-price">
                                    <span class="item-title">Mushroom Risotto</span>
                                    <span class="item-price">$25.00</span>
                                </div>
                                <p class="item-description">Creamy Arborio rice with wild mushrooms, parmesan, and truffle oil.</p>
                            </div>
                            <div class="menu-item">
                                <div class="item-title-price">
                                    <span class="item-title">Chicken Fried Rice</span>
                                    <span class="item-price">$30.00</span>
                                </div>
                                <p class="item-description">Classic fried rice with tender chicken, eggs, and mixed vegetables.</p>
                            </div>
                            <div class="menu-item">
                                <div class="item-title-price">
                                    <span class="item-title">Eggplant Parmesan</span>
                                    <span class="item-price">$40.00</span>
                                </div>
                                <p class="item-description">Layers of breaded eggplant, rich marinara, and melted mozzarella.</p>
                            </div>
                        </div>

                        <div class="menu-category">
                            <h2>Desserts</h2>
                            <div class="menu-item">
                                <div class="item-title-price">
                                    <span class="item-title">Tiramisu</span>
                                    <span class="item-price">$7.00</span>
                                </div>
                                <p class="item-description">Classic Italian coffee-flavored dessert with mascarpone cheese.</p>
                            </div>
                            <div class="menu-item">
                                <div class="item-title-price">
                                    <span class="item-title">Fruit Tart</span>
                                    <span class="item-price">$5.00</span>
                                </div>
                                <p class="item-description">Fresh seasonal fruits atop a sweet pastry cream in a crisp tart shell.</p>
                            </div>
                            <div class="menu-item">
                                <div class="item-title-price">
                                    <span class="item-title">CheeseCake</span>
                                    <span class="item-price">$10.00</span>
                                </div>
                                <p class="item-description">Creamy New York style cheesecake with a graham cracker crust.</p>
                            </div>
                            <div class="menu-item">
                                <div class="item-title-price">
                                    <span class="item-title">Apple Pie</span>
                                    <span class="item-price">$9.00</span>
                                </div>
                                <p class="item-description">Warm apple pie with a flaky crust, served with a scoop of vanilla ice cream.</p>
                            </div>
                            <div class="menu-item">
                                <div class="item-title-price">
                                    <span class="item-title">Chocolate Lava Cake</span>
                                    <span class="item-price">$8.00</span>
                                </div>
                                <p class="item-description">Decadent molten chocolate cake, served with a berry coulis.</p>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="menu-footer">
                    <p>www.himalayabliss.com</p>
                </div>
            </div>
        </div>
    </body>
    </html>

## FOR ADMINISTRATION PAGE(admins1.html):
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Administration & Collaborators</title>
        <style>
            
            body {
                font-family: Arial, sans-serif;
                margin: 0;
                padding: 40px 20px;
                background-color: #f7f7f7;  
                display: flex;
                flex-direction: column;
                align-items: center;
                min-height: 100vh;
            }

            
            .section-title {
                font-size: 2.2em;
                color: #333;
                margin-bottom: 50px;
                font-weight: 600;
                border-bottom: 3px solid #ccc;
                padding-bottom: 10px;
            }

            
            .collaborators-grid {
                display: flex;
                flex-wrap: wrap;
                justify-content: center;
                gap: 30px;
                max-width: 1000px;
            }

            
            .collaborator-card {
                background-color: #fff;
                border: 1px solid #ddd;
                border-radius: 8px;
                box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
                width: 300px;  
                overflow: hidden;
                transition: transform 0.3s;
            }

            .collaborator-card:hover {
                transform: translateY(-5px);
                box-shadow: 0 6px 15px rgba(0, 0, 0, 0.15);
            }

            
            .card-header {
                display: flex;
                align-items: center;
                padding: 20px 20px 10px 20px;
            }

            .collaborator-image {
                width: 70px;
                height: 70px;
                border-radius: 50%;
                overflow: hidden;
                margin-right: 15px;
                border: 3px solid #ffcc66; 
            }

            .collaborator-image img {
                width: 100%;
                height: 100%;
                object-fit: cover;
                display: block;
            }

            .collaborator-name {
                font-size: 1.4em;
                font-weight: bold;
                color: #333;
            }

            
            .collaborator-designation {
                padding: 10px 20px;
                color: white;
                font-weight: bold;
                text-transform: uppercase;
                font-size: 0.9em;
                margin-bottom: 5px;
            }

            
            .tag-orange {
                background-color: #ffaa33;  
            }
            .tag-blue {
                background-color: #33aaff;  
            }

            
            .collaborator-details {
                padding: 10px 20px 20px 20px;
                font-size: 0.9em;
                line-height: 1.5;
                color: #666;
            }

            
            @media (max-width: 650px) {
                .collaborators-grid {
                    flex-direction: column;
                    align-items: center;
                }
                .collaborator-card {
                    width: 90%;
                    max-width: 350px;
                }
            }
        </style>
    </head>
    <body>
        <h1 class="section-title">Administration & Collaborators</h1>

        <div class="collaborators-grid">
            
            <div class="collaborator-card">
                <div class="card-header">
                    <div class="collaborator-image">
                        <img src="Mark.webp" alt="Mark Zuckerberg">
                    </div>
                    <div class="collaborator-name">Mark Zuckerberg</div>
                </div>
                <div class="collaborator-designation tag-orange">
                    Chief Strategist
                </div>
                <div class="collaborator-details">
                    **Details:** Mr. Zuckerberg provides executive oversight on global platform integration and guides our long-term vision for community engagement and digital strategy.
                </div>
            </div>

            <div class="collaborator-card">
                <div class="card-header">
                    <div class="collaborator-image">
                        <img src="gates1.webp" alt="Bill Gates">
                    </div>
                    <div class="collaborator-name">Bill Gates</div>
                </div>
                <div class="collaborator-designation tag-blue">
                    Lead Technology Advisor
                </div>
                <div class="collaborator-details">
                    **Details:** Mr. Gates focuses on leveraging emerging technologies to enhance our operational efficiency and supports our initiatives in sustainable growth and resource management.
                </div>
            </div>

            <div class="collaborator-card">
                <div class="card-header">
                    <div class="collaborator-image">
                        <img src="jeff.webp" alt="Jeff Bezos">
                    </div>
                    <div class="collaborator-name">Jeff Bezos</div>
                </div>
                <div class="collaborator-designation tag-orange">
                    E-commerce & Logistics Partner
                </div>
                <div class="collaborator-details">
                    **Details:** Mr. Bezos collaborates on optimizing supply chain logistics and scaling operations across vast geographical markets with high-volume precision and reliability.
                </div>
            </div>
            
            <div class="collaborator-card">
                <div class="card-header">
                    <div class="collaborator-image">
                        <img src="ceo.jpg" alt="Veshwanth R">
                    </div>
                    <div class="collaborator-name">Veshwanth R</div>
                </div>
                <div class="collaborator-designation tag-blue">
                    Founder and CEO
                </div>
                <div class="collaborator-details">
                    **Details:** Founder and CEO of the restaurant HIMALAYA BLISS provides a fine dining restaurant as in top of the Multi-Cuisine Restaurant.
                </div>
            </div>

            <div class="collaborator-card">
                <div class="card-header">
                    <div class="collaborator-image">
                        <img src="joel.jpg" alt="Placeholder Admin">
                    </div>
                    <div class="collaborator-name">Joel Austin</div>
                </div>
                <div class="collaborator-designation tag-orange">
                    Head of Finance
                </div>
                <div class="collaborator-details">
                    **Details:** Responsible for all financial planning, reporting, and investor relations, ensuring robust fiscal health and transparency.
                </div>
            </div>
            
        </div>
    </body>
    </html>

## FOR CONTACTPAGE(contact.html):
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Contact Us - Modern Layout</title>
        <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
        
        <style>
        
            body {
                margin: 0;
                font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
                background-color: #2c3e50; 
                color: #ecf0f1; 
                display: flex;
                justify-content: center;
                align-items: center;
                min-height: 100vh;  
                overflow: auto;  
            }

            .contact-page-wrapper {
                width: 90%;
                max-width: 1200px;
                padding: 40px;
                background-color: #34495e;  
                border-radius: 10px;
                box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
                
                
                background-image: url('https://images.unsplash.com/photo-1519782800346-411a7741695f?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=M3w0NTMzNXwwfDF8c2VhcmNofDEzfHxjaXR5c2NhcGUlMjBkYXJrfGVufDB8fHx8MTcwOTI4NjkwMHww&ixlib=rb-4.0.3&q=80&w=1080'); 
                background-size: cover;
                background-position: center;
                background-repeat: no-repeat;
                position: relative;  
                z-index: 1;  
            }

            
            .contact-page-wrapper::before {
                content: '';
                position: absolute;
                top: 0;
                left: 0;
                right: 0;
                bottom: 0;
                background-color: rgba(0, 0, 0, 0.6);  
                border-radius: 10px;
                z-index: -1;  
            }

            
            .header-content {
                text-align: center;
                margin-bottom: 50px;
                color: #ffffff;  
            }

            .header-content h1 {
                font-size: 3em;
                margin-bottom: 15px;
            }

            .header-content p {
                font-size: 1.1em;
                line-height: 1.6;
                max-width: 800px;
                margin: 0 auto;
                color: #bdc3c7;  
            }

            
            .main-content-area {
                display: flex;
                flex-wrap: wrap;  
                gap: 40px;  
                justify-content: center;
            }

            
            .contact-details-column {
                flex: 1;  
                min-width: 300px;  
                padding: 20px;
                color: #ecf0f1;
            }

            .detail-item {
                display: flex;
                align-items: flex-start;  
                margin-bottom: 30px;
            }

            .icon-circle {
                width: 60px;
                height: 60px;
                border-radius: 50%;
                background-color: #ecf0f1;  
                color: #2c3e50;  
                display: flex;
                justify-content: center;
                align-items: center;
                font-size: 1.5em;
                margin-right: 20px;
                box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
            }

            .detail-text h3 {
                margin: 0 0 5px 0;
                font-size: 1.4em;
                color: #ffffff;
            }

            .detail-text p {
                margin: 0;
                font-size: 1em;
                line-height: 1.5;
                color: #bdc3c7;
            }

            
            .contact-form-column {
                flex: 1;  
                min-width: 350px;  
                background-color: #ffffff;  
                border-radius: 10px;
                padding: 40px;
                box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
                color: #2c3e50;  
            }

            .form-container h2 {
                text-align: center;
                margin-bottom: 30px;
                font-size: 2em;
                color: #34495e;
            }

            .form-group {
                margin-bottom: 25px;
            }

            .form-group input[type="text"],
            .form-group input[type="email"],
            .form-group textarea {
                width: 100%;
                padding: 12px 0;  
                border: none;  
                border-bottom: 1px solid #ccc;  
                font-size: 1.1em;
                color: #34495e;
                background-color: transparent;  
                box-sizing: border-box;  
                outline: none;  
            }

            .form-group input::placeholder,
            .form-group textarea::placeholder {
                color: #95a5a6;  
            }

            .form-group input:focus,
            .form-group textarea:focus {
                border-bottom-color: #3498db; 
            }

            .form-group textarea {
                resize: vertical;  
                min-height: 80px;
            }

            .send-button {
                width: 100%;
                padding: 15px;
                background-color: #1abc9c; 
                color: white;
                border: none;
                border-radius: 5px;
                font-size: 1.2em;
                cursor: pointer;
                transition: background-color 0.3s ease;
            }

            .send-button:hover {
                background-color: #16a085;  
            }

            
            @media (max-width: 768px) {
                .main-content-area {
                    flex-direction: column;  
                    gap: 20px;
                }

                .contact-page-wrapper {
                    padding: 30px;
                    width: 95%;
                }

                .header-content h1 {
                    font-size: 2.5em;
                }

                .header-content p {
                    font-size: 1em;
                }

                .contact-details-column,
                .contact-form-column {
                    min-width: unset;  
                    width: 100%;
                }
            }
        </style>
    </head>
    <body>
        <div class="contact-page-wrapper">
            <div class="header-content">
                <h1>Contact Us</h1>
                <p>For inquiries regarding **Food Quality, Hygiene, Sanitation, or Facility Maintenance**, please use the form below. We prioritize maintaining the highest standards of safety and operational excellence.</p>
            </div>

            <div class="main-content-area">
                <div class="contact-details-column">
                    <div class="detail-item">
                        <div class="icon-circle"><i class="fas fa-home"></i></div>
                        <div class="detail-text">
                            <h3>Address</h3>
                            <p>4871 Sugar Campcross Road,<br>Owatonna, Minnesota,<br>55060</p>
                        </div>
                    </div>
                    <div class="detail-item">
                        <div class="icon-circle"><i class="fas fa-phone-alt"></i></div>
                        <div class="detail-text">
                            <h3>Phone</h3>
                            <p>561-456-2321</p>
                        </div>
                    </div>
                    <div class="detail-item">
                        <div class="icon-circle"><i class="fas fa-envelope"></i></div>
                        <div class="detail-text">
                            <h3>Email</h3>
                            <p>himalayasbliss3@gmail.com</p>
                        </div>
                    </div>
                </div>

                <div class="contact-form-column">
                    <div class="form-container">
                        <h2>Send Message</h2>
                        <form>
                            <div class="form-group">
                                <input type="text" id="fullName" placeholder="Full Name">
                            </div>
                            <div class="form-group">
                                <input type="email" id="email" placeholder="Email">
                            </div>
                            <div class="form-group">
                                <textarea id="message" placeholder="Type your Message..." rows="5"></textarea>
                            </div>
                            <button type="submit" class="send-button">Send</button>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </body>
    </html>
## OUTPUT:
## FOR LOOKPAGE(restdesign.html):
![1](web1.png)
## FOR HOMEPAGE(home.html):
<img width="1918" height="1198" alt="web2" src="https://github.com/user-attachments/assets/f7372e26-e55c-49c0-ad67-62bcfe748b55" />

## FOR MENUPAGE(menus1.html):

<img width="1918" height="1198" alt="web3 1" src="https://github.com/user-attachments/assets/087a3254-7bc1-47e5-bb5d-3e9a414dd820" />

<img width="1917" height="1197" alt="web 3 2" src="https://github.com/user-attachments/assets/1698a6da-42dc-4d69-8a82-1b34de715cc6" />


## FOR ADMINISTRATION PAGE(admins1.html):

<img width="1916" height="1198" alt="web4" src="https://github.com/user-attachments/assets/e58b6c14-c8a0-4dfe-88f3-a334226e98ba" />

## FOR CONTACTPAGE(contact.html):

<img width="1918" height="1198" alt="web5" src="https://github.com/user-attachments/assets/804e7001-a43c-42c6-967b-518368ecbd07" />

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
