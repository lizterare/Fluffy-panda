<!DOCTYPE html>
<html lang="en">   
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fluffy Panda Milktea House</title>
    <link rel="shortcut icon" href="12.png">
    <link href="https://fonts.googleapis.com/css2?family=Quicksand:wght@400;600;700&family=Poppins:wght@300;400;500&display=swap" rel="stylesheet">

 <style>
    :root {
        --primary-color: #96BF8A; 
        --secondary-color: #F7E9C8; 
        --text-dark: #333;
        --text-light: #fff;
        --bg-dark-transparent: rgba(0, 0, 0, 0.85);
        --font-heading: 'Quicksand', sans-serif;
        --font-body: 'Poppins', sans-serif;
    }

    body {
        font-family: var(--font-body);
        margin: 0;
        padding: 0;
        scroll-behavior: smooth;
        background-color: var(--secondary-color);
    }

    html{
        scroll-behavior: smooth;
    }

    h1, h2, h3 {
        font-family: var(--font-heading);
        font-weight: 700;
        color: var(--text-light); 
    }

   nav {
      position: fixed;
      top: 0;
      width: 100%;
      background: var(--bg-dark-transparent);
      padding: 15px 0;
      z-index: 1000;
      box-shadow: 0 2px 10px rgba(0, 0, 0, 0.4);
    }

    .nav-container {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 0 20px;
    }

    .nav-left {
     display: flex;
     align-items: center;
     gap: 15px;
    }

    .logo {
     height: 45px;
     width: 45px;
     object-fit: cover;
    }

    .brand-name {
     color: var(--primary-color);
     font-weight: 700;
     font-size: 1.8rem;
     margin: 0;
     letter-spacing: 1px;
    }

    .nav-right a {
     color: var(--text-light);
     margin-left: 25px;
     text-decoration: none;
     font-weight: 500;
     transition: color 0.3s ease;
    }

    .nav-right a:hover {
     color: var(--primary-color);
     text-decoration: none;
    }

    section {
        min-height: 100vh; 
        display: flex;
        justify-content: center;
        align-items: center;
        text-align: center;
        padding: 100px 20px 20px;
        background-size: cover;
        background-position: center;
        background-attachment: fixed;
        color: var(--text-light);
    }

   section .overlay {
    margin: 0;
    background: rgba(0, 0, 0, 0.6);
    padding: 80px 0;
    width: 100vw;
    border-radius: 0;
    box-shadow: 0 0 30px rgba(0, 0, 0, 0.5);
    position: relative;
    left: 50%;
    transform: translateX(-50%);
}

    section, div{
        margin: -0;
        padding: 0;
    }

    #section1, #section2, #section3, #section4, #section5 {
         background-image: linear-gradient(rgba(0, 0, 0, 1), rgba(0, 0, 0, 0.7)), url("123.jpg");
    }

    #section1 h1 {
        font-size: 4.5rem;
        color: var(--primary-color);
        text-shadow: 2px 2px #000;
    }

    #section2 h2, #section3 h2, #section4 h1 {
        font-size: 3rem;
        margin-bottom: 25px;
        color: var(--primary-color);
    }
    
    #section4 h3 {
        color: var(--text-light);
        font-size: 1.2rem;
        font-weight: 300;
        line-height: 1.8;
    }

    #section2 p {
        line-height: 1.8;
        font-size: 1.2rem;
        font-weight: 300;
    }

    .grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    gap: 30px; 
    margin-top: 40px;
    padding: 0 60px; 
    box-sizing: border-box;
    }


    .product {
        display: flex;
        flex-direction: column;
        background: var(--text-light); 
        border: 2px solid var(--primary-color);
        border-radius: 12px;
        padding: 20px 20px;
        box-shadow: 0 4px 12px rgba(0,0,0,0.1);
        transition: transform 0.4s ease, box-shadow 0.4s ease;
        color: var(--text-dark);
        text-decoration: none;
        overflow: hidden;
    }

    .product img {
        width: 100%;      
        height: 250px; 
        object-fit: cover; 
        border-radius: 8px;
        margin-bottom: 15px;
        transition: transform 0.4s ease;
    }

    .product-info {
        text-align: center;
    }

    .product h3 {
        margin: 0;
        font-size: 1.4rem;
        color: var(--text-dark);
        transition: color 0.3s ease;
    }

    .product:hover {
        transform: translateY(-8px);
        box-shadow: 0 12px 25px rgba(0,0,0,0.25);
        background: var(--secondary-color);
    }

    .product:hover img {
        transform: scale(1.05); 
    }

    .product:hover h3 {
        color: var(--primary-color);
    }
    
    #section5 h1 {
        font-size: 2rem;
        font-weight: 400;
        margin: 15px 0;
    }
    
    #section5 h1:first-of-type {
        color: var(--primary-color);
        font-weight: 600;
        font-size: 3rem;
    }

    footer {
        text-align: center;
        padding: 25px;
        background: var(--bg-dark-transparent);
        color: var(--primary-color);
        font-size: 1rem;
        font-weight: 500;
    }

    @media (max-width: 768px) {
  .grid {
    padding: 0 20px;
        } 
    }

    @media (max-width: 768px) {
        #section1 h1 {
            font-size: 3.5rem;
        }

        #section2 h2, #section3 h2, #section4 h1 {
            font-size: 2.2rem;
        }

        .nav-right a {
            margin-left: 10px;
            font-size: 0.9rem;
        }
    }
</style>
</head>
<body>

    <nav>
  <div class="nav-container">
    <div class="nav-left">
      <img src="12.png" alt="Fluffy Panda Logo" class="logo">
      <h3 class="brand-name">FLUFFY PANDA</h3>
    </div>
    <div class="nav-right">
      <a href="#section1">Home</a>
      <a href="#section2">About</a>
      <a href="#section3">Menu</a>
      <a href="#section4">Why Us</a>
      <a href="#section5">Contact</a>
    </div>
  </div>
</nav>

    <section id="section1">
        <div class="overlay">
            <h1>Welcome to Fluffy Panda</h1>
            <h2>Your Cozy Spot for Milktea & Snacks</h2>
        </div>
    </section>

    <section id="section2">
        <div class="overlay">
            <h2>Our Story</h2>
            <p>
                Fluffy Panda is more than just a milk tea house—it's a cozy gathering spot. 
                Conveniently located in front of Star Elementary beside Bagong Silang High School, 
                we're known for our best-selling milk tea. We've expanded our menu to offer a delightful 
                range of snacks, including fries and hotdogs, alongside variations of milk tea, 
                ice cream, and coffee-based flavors to satisfy every craving.
            </p>
        </div>
    </section>

    <section id="section3">
        <div class="overlay">
            <h2>Menu Highlights</h2>
            <div class="grid">
                <a href="product1.html" class="product">
                    <img src="mt.jpg" alt="Milk Tea">
                    <div class="product-info">
                        <h3>Milk Tea</h3>
                    </div>
                </a> 

                <a href="product2.html" class="product">
                    <img src="F1.jpg" alt="Frappe">
                    <div class="product-info">
                        <h3>Frappe</h3>
                    </div>
                </a>

                <a href="product3.html" class="product">
                    <img src="ic0.jpg" alt="Iced Coffee">
                    <div class="product-info">
                        <h3>Iced Coffee</h3>
                    </div>
                </a>

                <a href="product4.html" class="product">
                    <img src="ft0.jpg" alt="Fruit Tea">
                    <div class="product-info">
                        <h3>Fruit Tea</h3>
                    </div>
                </a>

                <a href="product5.html" class="product">
                    <img src="sh11.jpg" alt="Shake">
                    <div class="product-info">
                        <h3>Shake</h3>
                    </div>
                </a>

                <a href="product6.html" class="product">
                    <img src="sd0.jpg" alt="Fruit Soda Drinks">
                    <div class="product-info">
                        <h3>Fruit Soda Drinks</h3>
                    </div>
                </a>

                <a href="product7.html" class="product">
                    <img src="ms0.jpg" alt="Milk Shake">
                    <div class="product-info">
                        <h3>Milk Shake</h3>
                    </div>
                </a>

                <a href="product8.html" class="product">
                    <img src="sn0.jpg" alt="Snacks">
                    <div class="product-info">
                        <h3>Snacks</h3>
                    </div>
                </a>
            </div>
        </div>
    </section>

    <section id="section4">
        <div class="overlay">
            <h1>Why Choose Us?</h1>
            <h3>
                Fluffy Panda is a modern milk tea shop designed for comfort and quality.
                Our goal is to provide a relaxing atmosphere where customers can enjoy 
                high-quality milk tea, delicious snacks, and great company. We focus on 
                variety and value to make every visit worthwhile.
            </h3>
        </div>
    </section>

    <section id="section5">
        <div class="overlay">
             <h1>Get In Touch</h1>
            <h1>Visit our FB Page: Fluffy Panda Milktea House</h1>
            <h1>Location: Right in front of Star Elementary School</h1>
            <h1>Contact: 09679470170</h1>
        </div>
    </section>

    <footer>
        © 2025 Fluffy Panda Milktea House. All rights reserved.
    </footer>

</body>
</html>
