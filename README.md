# Ex02 Commercial Website
## Date:12.08.2025

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

## PROGRAM
```

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Amazon Product Showcase</title>
    <style>
        /* Global Styles */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background: #f4f4f4;
            text-align: center;
        }

        /* Header */
        header {
            background: #ff9900;
            color: rgb(133, 97, 97);
            padding: 20px;
        }

        header h1 {
            margin: 15;
        }

        nav {
            margin-top: 10px;
        }

        nav a {
            color: white;
            margin: 0 10px;
            text-decoration: none;
            font-size: 18px;
        }

        nav a:hover {
            text-decoration: underline;
        }

        /* Sections */
        .section {
            padding: 50px 20px;
            background: white;
            margin: 20px auto;
            width: 80%;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            display: none; /* Hide all sections initially */
        }

        /* Show only the active section */
        .active {
            display: block;
        }

        /* Product Section */
        .product-container {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
        }

        .product {
            background: #fff;
            padding: 15px;
            border-radius: 10px;
            width: 200px;
            text-align: center;
            margin: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s;
        }

        .product img {
            width: 100%;
            border-radius: 10px;
        }

        .product:hover {
            transform: scale(1.05);
        }

        /* Footer */
        footer {
            background: #333;
            color: white;
            padding: 10px 0;
            margin-top: 20px;
        }

        .social-links a {
            color: white;
            margin: 0 10px;
            text-decoration: none;
        }

        .social-links a:hover {
            text-decoration: underline;
        }
    </style>
</head>

<body>
    <!-- Header -->
    <header>
        <h1>Amazon Product Showcase</h1>
        <nav>
            <a href="#" onclick="showSection('home')">Home</a>
            <a href="#" onclick="showSection('products')">Products</a>
            <a href="#" onclick="showSection('about')">About Us</a>
            <a href="#" onclick="showSection('contact')">Contact</a>
        </nav>
    </header>

    <!-- Home Section -->
    <section id="home" class="section active">
        <h2>Welcome to Our Amazon Product Showcase</h2>
        <p>Explore the best grooming and personal care products from Amazon, selected just for you!</p>
    </section>

    <!-- Products Section -->
    <section id="products" class="section">
        <h2>Our Featured Products</h2>
        <div class="product-container">
            <!-- Product 1 - Hair Serum -->
            <div class="product">
                <img src="hairserum.png" alt="Hair Serum">
                <h3>Hair Serum</h3>
                <p>Protects hair from damage and adds shine. Ideal for frizz control.</p>
                <p><strong>Price:</strong> ₹399</p>
            </div>

            <!-- Product 2 - Face Wash -->
            <div class="product">
                <img src="facewash.png" alt="Face Wash">
                <h3>Face Wash</h3>
                <p>Gently cleanses and removes impurities for glowing skin.</p>
                <p><strong>Price:</strong> ₹299</p>
            </div>


            <!-- Product 3 - Hair Dryer -->
            <div class="product">
                <img src="hairdryer.png" alt="Hair Dryer">
                <h3>Hair Dryer</h3>
                <p>Fast and efficient drying for salon-like results.</p>
                <p><strong>Price:</strong> ₹1,299</p>
            </div>
        </div>
    </section>

    <!-- About Us Section -->
    <section id="about" class="section">
        <h2>About Us</h2>
        <p>We curate the best Amazon products to make your shopping easier and smarter.</p>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="section">
        <h2>Contact Us</h2>
        <p>Email: support@amazonshowcase.com</p>
        <p>Phone: +91-9876543210</p>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; <span id="year"></span> Amazon Product Showcase. All rights reserved.</p>
        <div class="social-links">
            <a href="#">Facebook</a> |
            <a href="#">Twitter</a> |
            <a href="#">Instagram</a>
        </div>
    </footer>

    <!-- JavaScript -->
    <script>
        // Set current year in footer
        document.getElementById('year').innerText = new Date().getFullYear();

        // Function to show only one section at a time
        function showSection(sectionId) {
            // Hide all sections
            const sections = document.querySelectorAll('.section');
            sections.forEach(section => {
                section.classList.remove('active');
            });

            // Show the selected section
            document.getElementById(sectionId).classList.add('active');
        }
    </script>
</body>

</html>
```


## OUTPUT
<img width="1917" height="1072" alt="Screenshot 2025-08-12 222059" src="https://github.com/user-attachments/assets/8ca2fda0-2365-4317-bc49-7e927039d687" />
<img width="1917" height="1077" alt="Screenshot 2025-08-12 222115" src="https://github.com/user-attachments/assets/4d37c203-0115-4c67-8888-ffafc0a08b02" />
<img width="1915" height="1079" alt="Screenshot 2025-08-12 222129" src="https://github.com/user-attachments/assets/4b8ac035-5e55-4a17-8906-c4697632d93c" />
<img width="1919" height="1079" alt="Screenshot 2025-08-12 222141" src="https://github.com/user-attachments/assets/74763909-0381-442d-9535-f30d93c5fb6f" />




## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
