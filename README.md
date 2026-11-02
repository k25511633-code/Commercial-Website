# Commercial-Website
# Ex02 Commercial Website
## Date:31/10/2026

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.
## Devoleped by: Kaviya R
## Reg No: 212225040179
## PROGRAM
## HTML
```c

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>FragranceLux - Luxury Perfumes</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
</head>
<body>

    <!-- Header -->
    <header class="header">
        <div class="logo">
            <i class="fa-solid fa-spray-can-sparkles"></i>
            <div>
                <h2>FragranceLux</h2>
                <p>Live Elegant. Smell Divine.</p>
            </div>
        </div>

        <nav>
            <a href="#" class="active">Home</a>
            <a href="#categories">Shop <i class="fa-solid fa-chevron-down"></i></a>
            <a href="#about">About</a>
            <a href="#offers">Offers</a>
            <a href="#contact">Contact</a>
        </nav>

        <div class="header-icons">
            <input type="text" placeholder="Search perfumes...">
            <i class="fa-regular fa-user"></i>
            <i class="fa-solid fa-cart-shopping"></i>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="hero-content">
            <p class="small-title">DISCOVER YOUR FRAGRANCE</p>
            <h1>Our Signature Collection</h1>
            <p class="tagline">Luxury fragrances for every moment.</p>
            <a href="#categories" class="shop-btn">
                Shop Now <i class="fa-solid fa-arrow-right"></i>
            </a>
        </div>
    </section>

    <!-- Services -->
    <section class="services" id="about">

        <div class="service">
            <i class="fa-solid fa-truck-fast"></i>
            <div>
                <h3>Free Shipping</h3>
                <p>On orders above ₹999</p>
            </div>
        </div>

        <div class="service">
            <i class="fa-solid fa-shield-halved"></i>
            <div>
                <h3>Secure Payment</h3>
                <p>100% Secure & Trusted</p>
            </div>
        </div>

        <div class="service">
            <i class="fa-solid fa-gift"></i>
            <div>
                <h3>Special Offers</h3>
                <p>Save More, Smell Better</p>
            </div>
        </div>

        <div class="service">
            <i class="fa-solid fa-headset"></i>
            <div>
                <h3>24/7 Support</h3>
                <p>We're here to help</p>
            </div>
        </div>

    </section>

    <!-- Categories -->
    <section class="categories" id="categories">

        <h2 class="section-title">Shop by Category</h2>

        <div class="category-container">

            <div class="category-card">
                <img src="https://images.unsplash.com/photo-1594035910387-fea47794261f?w=600" alt="Men Perfume">
                <div class="category-name">
                    <h3>For Men</h3>
                    <i class="fa-solid fa-arrow-right"></i>
                </div>
            </div>

            <div class="category-card">
                <img src="https://images.unsplash.com/photo-1541643600914-78b084683601?w=600" alt="Women Perfume">
                <div class="category-name">
                    <h3>For Women</h3>
                    <i class="fa-solid fa-arrow-right"></i>
                </div>
            </div>

            <div class="category-card">
                <img src="https://images.unsplash.com/photo-1592945403244-b3fbafd7f539?w=600" alt="Unisex Perfume">
                <div class="category-name">
                    <h3>Unisex</h3>
                    <i class="fa-solid fa-arrow-right"></i>
                </div>
            </div>

            <div class="category-card">
                 <img src="https://www.adipec.com.br/uploads/news/68965113d40c3.jpg" alt="Premium Perfume">
                <div class="category-name">
                    <h3>Premium</h3>
                    <i class="fa-solid fa-arrow-right"></i>
                </div>
            </div>

            <div class="category-card">
                 <img src="https://images.unsplash.com/photo-1595425970377-c9703cf48b6d?w=600" alt="Luxury Perfume">
                <div class="category-name">
                    <h3>Luxury</h3>
                    <i class="fa-solid fa-arrow-right"></i>
                </div>
            </div>

        </div>
    </section>

    <!-- Offer Banner -->
    <section class="offer" id="offers">
        <div class="offer-text">
            <p>Get Up to</p>
            <h2>50% OFF</h2>
        </div>

        <div class="offer-description">
            <p>On Selected Fragrances</p>
            <a href="#categories">
                Shop the Deal <i class="fa-solid fa-arrow-right"></i>
            </a>
        </div>
    </section>

    <!-- Footer -->
    <footer id="contact">
        <h2>FragranceLux</h2>
        <p>Discover your signature fragrance with us.</p>
        <p>© 2026 FragranceLux. All Rights Reserved.</p>
    </footer>

</body>
</html>

```
## CSS
```c

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: Arial, sans-serif;
    background: #fff2e2;
    color: #49230f;
}

/* Header */
.header {
    width: 100%;
    min-height: 75px;
    padding: 10px 6%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    background: #fff8ee;
    border-bottom: 1px solid #e6c9a9;
}

.logo {
    display: flex;
    align-items: center;
    gap: 12px;
}

.logo > i {
    font-size: 38px;
    color: #8b351e;
}

.logo h2 {
    font-family: Georgia, serif;
    font-size: 27px;
}

.logo p {
    font-size: 12px;
    margin-top: 3px;
}

nav {
    display: flex;
    align-items: center;
    gap: 28px;
}

nav a {
    text-decoration: none;
    color: #49230f;
    font-weight: bold;
    font-size: 15px;
    padding: 10px 13px;
}

nav a:hover,
nav .active {
    background: #870d20;
    color: white;
    border-radius: 8px;
}

.header-icons {
    display: flex;
    align-items: center;
    gap: 23px;
}

.header-icons input {
    width: 190px;
    padding: 11px 15px;
    border: 1px solid #dfc4a6;
    border-radius: 25px;
    background: transparent;
    outline: none;
}

.header-icons i {
    font-size: 23px;
    cursor: pointer;
}

/* Hero */
.hero {
    min-height: 340px;
    background:
        linear-gradient(90deg, rgba(255,225,191,0.35), rgba(255,225,191,0.05)),
        url("https://images.unsplash.com/photo-1594035910387-fea47794261f?w=1800")
        center 45% / cover no-repeat;
    display: flex;
    align-items: center;
    padding: 45px 9%;
}

.hero-content {
    max-width: 750px;
}

.small-title {
    font-size: 14px;
    letter-spacing: 5px;
    font-weight: bold;
    margin-bottom: 18px;
}

.hero h1 {
    font-family: Georgia, serif;
    font-size: clamp(36px, 5vw, 65px);
    margin-bottom: 12px;
}

.tagline {
    font-family: Georgia, serif;
    font-style: italic;
    font-size: 27px;
    margin-bottom: 28px;
}

.shop-btn {
    display: inline-block;
    background: #870d20;
    color: white;
    padding: 14px 28px;
    border-radius: 30px;
    text-decoration: none;
    font-weight: bold;
}

.shop-btn i {
    margin-left: 10px;
}

.shop-btn:hover {
    background: #50100d;
}

/* Services */
.services {
    
    margin: 15px 5%;
    padding: 18px;
    background: #fcebd7;
    border-radius: 15px;
    display: grid;
    grid-template-columns: repeat(4, 1fr);
}

.service {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 17px;
    border-right: 1px solid #dfc6a7;
    padding: 5px;
}

.service:last-child {
    border: none;
}

.service i {
    font-size: 35px;
}

.service h3 {
    font-size: 16px;
    margin-bottom: 5px;
}

.service p {
    font-size: 12px;
}

/* Categories */
.categories {
    padding: 15px 5% 35px;
}

.section-title {
    text-align: center;
    font-family: Georgia, serif;
    font-size: 34px;
    margin-bottom: 22px;
}

.category-container {
    display: grid;
    grid-template-columns: repeat(5, 1fr);
    gap: 18px;
}

.category-card {
    background: #fff0dd;
    border-radius: 12px;
    overflow: hidden;
    border: 1px solid #e6cdb2;
    box-shadow: 0 3px 8px rgba(80, 40, 10, 0.1);
    transition: 0.3s;
}

.category-card:hover {
    transform: translateY(-7px);
    box-shadow: 0 8px 18px rgba(80, 40, 10, 0.2);
}

.category-card img {
    width: 100%;
    height: 135px;
    object-fit: cover;
    display: block;
}

.category-name {
    padding: 13px 16px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.category-name h3 {
    font-size: 16px;
}

.category-name i {
    background: #54270f;
    color: white;
    padding: 9px;
    border-radius: 50%;
    font-size: 13px;
}

/* Offer Banner */
.offer {
    margin: 0 3% 30px;
    min-height: 115px;
    padding: 15px 13%;
    border-radius: 18px;
    background:
        linear-gradient(90deg, rgba(85,0,15,0.95), rgba(110,0,20,0.75)),
        url("https://images.unsplash.com/photo-1513201099705-a9746e1e201f?w=1500")
        center / cover;
    color: #ffe0a0;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.offer-text p {
    font-family: Georgia, serif;
    font-size: 24px;
    font-style: italic;
}

.offer-text h2 {
    font-family: Georgia, serif;
    font-size: 48px;
}

.offer-description {
    display: flex;
    align-items: center;
    gap: 30px;
}

.offer-description p {
    font-family: Georgia, serif;
    font-size: 23px;
    font-style: italic;
}

.offer-description a {
    background: #ffecd1;
    color: #54230d;
    padding: 14px 24px;
    border-radius: 30px;
    text-decoration: none;
    font-weight: bold;
    white-space: nowrap;
}

/* Footer */
footer {
    background: #54230f;
    color: #fff0dd;
    text-align: center;
    padding: 25px;
}

footer h2 {
    font-family: Georgia, serif;
    margin-bottom: 8px;
}

footer p {
    margin: 8px;
    font-size: 13px;
}

/* Responsive Design */
@media (max-width: 1000px) {
    .header {
        flex-wrap: wrap;
        gap: 15px;
    }

    nav {
        gap: 8px;
    }

    .category-container {
        grid-template-columns: repeat(3, 1fr);
    }

    .services {
        grid-template-columns: repeat(2, 1fr);
        gap: 15px;
    }

    .service:nth-child(2) {
        border-right: none;
    }

    .offer {
        padding: 20px 5%;
    }
}

@media (max-width: 600px) {
    .header {
        justify-content: center;
    }

    nav {
        flex-wrap: wrap;
        justify-content: center;
    }

    .header-icons input {
        width: 150px;
    }

    .hero {
        min-height: 300px;
        padding: 30px 6%;
    }

    .hero h1 {
        font-size: 36px;
    }

    .tagline {
        font-size: 20px;
    }

    .services {
        grid-template-columns: 1fr;
    }

    .service {
        justify-content: flex-start;
        border-right: none;
        border-bottom: 1px solid #dfc6a7;
        padding: 12px;
    }

    .category-container {
        grid-template-columns: repeat(2, 1fr);
        gap: 12px;
    }

    .category-card img {
        height: 120px;
    }

    .section-title {
        font-size: 27px;
    }

    .offer {
        flex-direction: column;
        text-align: center;
        gap: 15px;
    }

    .offer-description {
        flex-direction: column;
        gap: 15px;
    }

    .offer-text h2 {
        font-size: 40px;
    }
}
```
## OUTPUT

![alt text](<Screenshot 2026-11-02 223313.png>)
![alt text](<Screenshot 2026-11-02 223342.png>)
## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
