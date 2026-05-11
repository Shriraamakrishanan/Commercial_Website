# Ex02 Commercial Website
## Date:

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
# index.html
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="LUXE - Premium e-commerce platform for curated lifestyle products">
    <title>LUXE - Premium Lifestyle Products</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600;700;800&family=Lato:wght@300;400;500;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- ===== NAVIGATION BAR ===== -->
    <nav class="navbar">
        <div class="navbar-container">
            <!-- Logo -->
            <div class="logo">
                <span class="logo-text">LUXE</span>
                <span class="logo-subtitle">Curated Collections</span>
            </div>

            <!-- Mobile Menu Toggle -->
            <button class="menu-toggle" id="menuToggle" aria-label="Toggle navigation menu">
                <span class="hamburger"></span>
            </button>

            <!-- Navigation Links -->
            <ul class="nav-menu" id="navMenu">
                <li><a href="#home" class="nav-link">Home</a></li>
                <li><a href="#products" class="nav-link">Collections</a></li>
                <li><a href="#about" class="nav-link">About</a></li>
                <li><a href="#contact" class="nav-link">Contact</a></li>
            </ul>

            <!-- CTA Button -->
            <div class="nav-cta">
                <button class="btn btn-secondary" id="cartBtn">Cart (0)</button>
            </div>
        </div>
    </nav>

    <!-- ===== HERO SECTION ===== -->
    <section class="hero" id="home">
        <div class="hero-container">
            <div class="hero-content">
                <h1 class="hero-title">Discover Timeless Elegance</h1>
                <p class="hero-subtitle">Handcrafted collections of premium lifestyle products</p>
                <button class="btn btn-primary" id="shopBtn">Explore Collections</button>
            </div>
            <div class="hero-image">
                <div class="hero-visual"></div>
            </div>
        </div>
    </section>

    <!-- ===== FEATURED PRODUCTS SECTION ===== -->
    <section class="featured" id="products">
        <div class="container">
            <div class="section-header">
                <h2 class="section-title">Featured Collections</h2>
                <p class="section-description">Curated selections from our finest artisans</p>
            </div>

            <!-- Products Grid -->
            <div class="products-grid">
                <!-- Product Card 1 -->
                <article class="product-card" data-product-id="001">
                    <div class="product-image">
                        <img src="images/leather-jacket.png" alt="Artisan Leather Jacket" class="product-img">
                        <span class="product-badge">New</span>
                    </div>
                    <div class="product-info">
                        <h3 class="product-name">Artisan Leather Jacket</h3>
                        <p class="product-category">Fashion</p>
                        <div class="product-rating">
                            <span class="stars">★★★★★</span>
                            <span class="rating-count">(124)</span>
                        </div>
                        <div class="product-footer">
                            <span class="product-price">$349.00</span>
                            <button class="btn-icon add-to-cart" aria-label="Add to cart">→</button>
                        </div>
                    </div>
                </article>

                <!-- Product Card 2 -->
                <article class="product-card" data-product-id="002">
                    <div class="product-image">
                        <img src="images/minimalist-watch.png" alt="Minimalist Watch" class="product-img">
                        <span class="product-badge sale">Sale</span>
                    </div>
                    <div class="product-info">
                        <h3 class="product-name">Minimalist Watch</h3>
                        <p class="product-category">Accessories</p>
                        <div class="product-rating">
                            <span class="stars">★★★★☆</span>
                            <span class="rating-count">(89)</span>
                        </div>
                        <div class="product-footer">
                            <span class="product-price">$189.00</span>
                            <button class="btn-icon add-to-cart" aria-label="Add to cart">→</button>
                        </div>
                    </div>
                </article>

                <!-- Product Card 3 -->
                <article class="product-card" data-product-id="003">
                    <div class="product-image">
                        <img src="images/cotton-hoodie.png" alt="Organic Cotton Hoodie" class="product-img">
                    </div>
                    <div class="product-info">
                        <h3 class="product-name">Organic Cotton Hoodie</h3>
                        <p class="product-category">Apparel</p>
                        <div class="product-rating">
                            <span class="stars">★★★★★</span>
                            <span class="rating-count">(156)</span>
                        </div>
                        <div class="product-footer">
                            <span class="product-price">$129.00</span>
                            <button class="btn-icon add-to-cart" aria-label="Add to cart">→</button>
                        </div>
                    </div>
                </article>

                <!-- Product Card 4 -->
                <article class="product-card" data-product-id="004">
                    <div class="product-image">
                        <img src="images/coffee-set.png" alt="Artisan Coffee Set" class="product-img">
                        <span class="product-badge hot">Trending</span>
                    </div>
                    <div class="product-info">
                        <h3 class="product-name">Artisan Coffee Set</h3>
                        <p class="product-category">Home & Decor</p>
                        <div class="product-rating">
                            <span class="stars">★★★★★</span>
                            <span class="rating-count">(203)</span>
                        </div>
                        <div class="product-footer">
                            <span class="product-price">$299.00</span>
                            <button class="btn-icon add-to-cart" aria-label="Add to cart">→</button>
                        </div>
                    </div>
                </article>
            </div>

            <!-- View All Button -->
            <div class="view-all">
                <button class="btn btn-outline">View All Products</button>
            </div>
        </div>
    </section>

    <!-- ===== BENEFITS SECTION ===== -->
    <section class="benefits">
        <div class="container">
            <div class="benefits-grid">
                <div class="benefit-card">
                    <div class="benefit-icon">🚚</div>
                    <h3>Free Shipping</h3>
                    <p>On orders over $100 worldwide</p>
                </div>
                <div class="benefit-card">
                    <div class="benefit-icon">🛡️</div>
                    <h3>Secure Payment</h3>
                    <p>100% encrypted transactions</p>
                </div>
                <div class="benefit-card">
                    <div class="benefit-icon">↩️</div>
                    <h3>Easy Returns</h3>
                    <p>30-day money-back guarantee</p>
                </div>
                <div class="benefit-card">
                    <div class="benefit-icon">💬</div>
                    <h3>24/7 Support</h3>
                    <p>Dedicated customer service team</p>
                </div>
            </div>
        </div>
    </section>

    <!-- ===== ABOUT SECTION ===== -->
    <section class="about" id="about">
        <div class="container">
            <div class="about-content">
                <div class="about-text">
                    <h2 class="section-title">About LUXE</h2>
                    <p>We believe that exceptional products deserve exceptional stories. Since 2015, LUXE has been connecting discerning customers with the world's finest artisans and craftspeople.</p>
                    <p>Each item in our collection is handpicked for quality, authenticity, and timeless appeal. We partner exclusively with creators who share our commitment to sustainable practices and ethical production.</p>
                    <div class="about-stats">
                        <div class="stat">
                            <span class="stat-number">50K+</span>
                            <span class="stat-label">Happy Customers</span>
                        </div>
                        <div class="stat">
                            <span class="stat-number">200+</span>
                            <span class="stat-label">Artisan Partners</span>
                        </div>
                        <div class="stat">
                            <span class="stat-number">98%</span>
                            <span class="stat-label">Satisfaction Rate</span>
                        </div>
                    </div>
                </div>
                <div class="about-visual">
                    <div class="about-image"></div>
                </div>
            </div>
        </div>
    </section>

    <!-- ===== NEWSLETTER SECTION ===== -->
    <section class="newsletter">
        <div class="container">
            <div class="newsletter-content">
                <h2>Stay Updated</h2>
                <p>Subscribe to receive exclusive offers and new collection announcements</p>
                <form class="newsletter-form" id="newsletterForm">
                    <input type="email" placeholder="Enter your email" required aria-label="Email address">
                    <button type="submit" class="btn btn-primary">Subscribe</button>
                </form>
                <p class="newsletter-disclaimer">We respect your privacy. Unsubscribe at any time.</p>
            </div>
        </div>
    </section>

    <!-- ===== FOOTER ===== -->
    <footer class="footer" id="contact">
        <div class="container">
            <!-- Footer Main Content -->
            <div class="footer-content">
                <!-- Company Info -->
                <div class="footer-section">
                    <h4>LUXE</h4>
                    <p>Premium curated collections for the discerning lifestyle.</p>
                    <div class="social-links">
                        <a href="#" aria-label="Instagram">Instagram</a>
                        <a href="#" aria-label="Facebook">Facebook</a>
                        <a href="#" aria-label="Twitter">Twitter</a>
                    </div>
                </div>

                <!-- Quick Links -->
                <div class="footer-section">
                    <h4>Shop</h4>
                    <ul>
                        <li><a href="#products">All Collections</a></li>
                        <li><a href="#">New Arrivals</a></li>
                        <li><a href="#">Sale Items</a></li>
                        <li><a href="#">Gift Guide</a></li>
                    </ul>
                </div>

                <!-- Support -->
                <div class="footer-section">
                    <h4>Support</h4>
                    <ul>
                        <li><a href="#">Contact Us</a></li>
                        <li><a href="#">FAQ</a></li>
                        <li><a href="#">Shipping Info</a></li>
                        <li><a href="#">Returns</a></li>
                    </ul>
                </div>

                <!-- Company -->
                <div class="footer-section">
                    <h4>Company</h4>
                    <ul>
                        <li><a href="#">About Us</a></li>
                        <li><a href="#">Careers</a></li>
                        <li><a href="#">Blog</a></li>
                        <li><a href="#">Press</a></li>
                    </ul>
                </div>
            </div>

            <!-- Footer Bottom -->
            <div class="footer-bottom">
                <div class="footer-left">
                    <p>&copy; 2024 LUXE. All rights reserved.</p>
                </div>
                <div class="footer-links">
                    <a href="#">Privacy Policy</a>
                    <a href="#">Terms of Service</a>
                    <a href="#">Cookie Settings</a>
                </div>
            </div>
        </div>
    </footer>

    <!-- Success Message (Initially Hidden) -->
    <div class="toast" id="toast"></div>

    <script src="scripts.js"></script>
</body>
</html>
```
# style.css
```css
/* ============================================
   LUXE - Professional E-Commerce Website
   Responsive Flexbox Layout
   ============================================ */

/* ===== CSS VARIABLES (Theme System) ===== */
:root {
    /* Colors */
    --primary-color: #1a1a1a;
    --secondary-color: #d4af37;
    --accent-color: #e8e8e8;
    --text-dark: #333333;
    --text-light: #666666;
    --bg-light: #fafafa;
    --bg-white: #ffffff;
    --border-color: #e0e0e0;
    --error-color: #e74c3c;
    --success-color: #2ecc71;

    /* Spacing */
    --spacing-xs: 0.5rem;
    --spacing-sm: 1rem;
    --spacing-md: 1.5rem;
    --spacing-lg: 2rem;
    --spacing-xl: 3rem;
    --spacing-2xl: 4rem;

    /* Typography */
    --font-display: 'Playfair Display', serif;
    --font-body: 'Lato', sans-serif;
    --font-size-base: 1rem;
    --font-size-sm: 0.875rem;
    --font-size-lg: 1.125rem;
    --font-size-xl: 1.5rem;
    --font-size-2xl: 2rem;
    --font-size-3xl: 3rem;

    /* Shadows */
    --shadow-sm: 0 2px 4px rgba(0, 0, 0, 0.05);
    --shadow-md: 0 4px 12px rgba(0, 0, 0, 0.1);
    --shadow-lg: 0 10px 30px rgba(0, 0, 0, 0.15);

    /* Transitions */
    --transition-base: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
    --transition-fast: all 0.15s ease-in-out;

    /* Border Radius */
    --radius-sm: 4px;
    --radius-md: 8px;
    --radius-lg: 12px;
}

/* ===== RESET & BASE STYLES ===== */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: var(--font-body);
    color: var(--text-dark);
    background-color: var(--bg-white);
    line-height: 1.6;
    overflow-x: hidden;
}

img {
    max-width: 100%;
    height: auto;
    display: block;
}

a {
    text-decoration: none;
    color: inherit;
}

button {
    border: none;
    cursor: pointer;
    font-family: inherit;
}

/* ===== CONTAINER LAYOUT ===== */
.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 var(--spacing-lg);
}

/* ===== NAVIGATION BAR (Flexbox) ===== */
.navbar {
    position: sticky;
    top: 0;
    z-index: 1000;
    background: var(--bg-white);
    border-bottom: 1px solid var(--border-color);
    padding: var(--spacing-md) 0;
    box-shadow: var(--shadow-sm);
}

.navbar-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 var(--spacing-lg);
}

.logo {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: var(--spacing-xs);
}

.logo-text {
    font-family: var(--font-display);
    font-size: 1.5rem;
    font-weight: 700;
    color: var(--primary-color);
    letter-spacing: 2px;
}

.logo-subtitle {
    font-size: 0.65rem;
    color: var(--secondary-color);
    font-weight: 500;
    letter-spacing: 1px;
    text-transform: uppercase;
}

/* Nav Menu - Flex Row (Desktop) */
.nav-menu {
    display: flex;
    gap: var(--spacing-xl);
    list-style: none;
    align-items: center;
}

.nav-link {
    font-size: var(--font-size-sm);
    font-weight: 500;
    color: var(--text-dark);
    position: relative;
    transition: var(--transition-fast);
}

.nav-link::after {
    content: '';
    position: absolute;
    bottom: -5px;
    left: 0;
    width: 0;
    height: 2px;
    background: var(--secondary-color);
    transition: width 0.3s ease;
}

.nav-link:hover::after {
    width: 100%;
}

.nav-cta {
    display: flex;
    gap: var(--spacing-md);
    align-items: center;
}

/* Mobile Menu Toggle - Hidden by default */
.menu-toggle {
    display: none;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 6px;
    background: transparent;
    padding: var(--spacing-sm);
}

.hamburger {
    width: 24px;
    height: 2px;
    background: var(--primary-color);
    transition: var(--transition-fast);
}

.menu-toggle.active .hamburger {
    background: var(--secondary-color);
}

/* ===== BUTTON STYLES ===== */
.btn {
    padding: 0.75rem 1.5rem;
    border-radius: var(--radius-md);
    font-size: var(--font-size-sm);
    font-weight: 600;
    transition: var(--transition-base);
    cursor: pointer;
    text-transform: uppercase;
    letter-spacing: 0.5px;
}

.btn-primary {
    background: var(--primary-color);
    color: var(--bg-white);
}

.btn-primary:hover {
    background: var(--secondary-color);
    color: var(--primary-color);
    transform: translateY(-2px);
    box-shadow: var(--shadow-md);
}

.btn-secondary {
    background: transparent;
    color: var(--text-dark);
    border: 1.5px solid var(--primary-color);
}

.btn-secondary:hover {
    background: var(--primary-color);
    color: var(--bg-white);
}

.btn-outline {
    background: transparent;
    color: var(--primary-color);
    border: 2px solid var(--primary-color);
}

.btn-outline:hover {
    background: var(--primary-color);
    color: var(--bg-white);
}

.btn-icon {
    width: 40px;
    height: 40px;
    border-radius: 50%;
    background: var(--primary-color);
    color: var(--bg-white);
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1.25rem;
    transition: var(--transition-base);
}

.btn-icon:hover {
    background: var(--secondary-color);
    color: var(--primary-color);
    transform: scale(1.1);
}

/* ===== HERO SECTION (Flexbox) ===== */
.hero {
    padding: var(--spacing-2xl) 0;
    background: linear-gradient(135deg, #f5f5f5 0%, #fafafa 100%);
    overflow: hidden;
}

.hero-container {
    display: flex;
    align-items: center;
    gap: var(--spacing-2xl);
    padding: var(--spacing-xl) var(--spacing-lg);
    max-width: 1200px;
    margin: 0 auto;
}

.hero-content {
    flex: 1;
    min-width: 300px;
    animation: slideInLeft 0.8s ease-out;
}

.hero-title {
    font-family: var(--font-display);
    font-size: var(--font-size-3xl);
    font-weight: 700;
    color: var(--primary-color);
    margin-bottom: var(--spacing-md);
    line-height: 1.2;
}

.hero-subtitle {
    font-size: var(--font-size-lg);
    color: var(--text-light);
    margin-bottom: var(--spacing-lg);
    font-weight: 300;
}

.hero-image {
    flex: 1;
    min-width: 300px;
}

.hero-visual {
    width: 100%;
    aspect-ratio: 1;
    border-radius: var(--radius-lg);
    background: linear-gradient(135deg, #d4af37 0%, #f4d03f 50%, #d4af37 100%);
    animation: slideInRight 0.8s ease-out;
    box-shadow: var(--shadow-lg);
}

/* ===== FEATURED PRODUCTS SECTION ===== */
.featured {
    padding: var(--spacing-2xl) 0;
    background: var(--bg-white);
}

.section-header {
    text-align: center;
    margin-bottom: var(--spacing-2xl);
}

.section-title {
    font-family: var(--font-display);
    font-size: var(--font-size-3xl);
    font-weight: 700;
    color: var(--primary-color);
    margin-bottom: var(--spacing-md);
}

.section-description {
    font-size: var(--font-size-lg);
    color: var(--text-light);
    font-weight: 300;
}

/* Products Grid - Flexbox */
.products-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: var(--spacing-xl);
    margin-bottom: var(--spacing-2xl);
}

/* Product Card - Flexbox for internal layout */
.product-card {
    background: var(--bg-white);
    border-radius: var(--radius-lg);
    overflow: hidden;
    box-shadow: var(--shadow-sm);
    transition: var(--transition-base);
    display: flex;
    flex-direction: column;
}

.product-card:hover {
    box-shadow: var(--shadow-lg);
    transform: translateY(-8px);
}

.product-image {
    position: relative;
    width: 100%;
    aspect-ratio: 1;
    overflow: hidden;
    background: var(--bg-light);
}

.image-placeholder {
    width: 100%;
    height: 100%;
    transition: transform 0.5s ease;
}

.product-card:hover .image-placeholder {
    transform: scale(1.05);
}

.product-img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: transform 0.5s ease;
    display: block;
}

.product-card:hover .product-img {
    transform: scale(1.05);
}

.gradient-1 { background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); }
.gradient-2 { background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%); }
.gradient-3 { background: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%); }
.gradient-4 { background: linear-gradient(135deg, #43e97b 0%, #38f9d7 100%); }

.product-badge {
    position: absolute;
    top: var(--spacing-md);
    right: var(--spacing-md);
    background: var(--primary-color);
    color: var(--bg-white);
    padding: 0.4rem 0.8rem;
    border-radius: var(--radius-sm);
    font-size: var(--font-size-sm);
    font-weight: 600;
    text-transform: uppercase;
}

.product-badge.sale {
    background: var(--error-color);
}

.product-badge.hot {
    background: var(--secondary-color);
    color: var(--primary-color);
}

.product-info {
    padding: var(--spacing-lg);
    display: flex;
    flex-direction: column;
    flex: 1;
}

.product-name {
    font-family: var(--font-display);
    font-size: 1.1rem;
    font-weight: 600;
    color: var(--primary-color);
    margin-bottom: var(--spacing-xs);
}

.product-category {
    font-size: var(--font-size-sm);
    color: var(--text-light);
    margin-bottom: var(--spacing-md);
    text-transform: uppercase;
    letter-spacing: 0.5px;
}

.product-rating {
    display: flex;
    align-items: center;
    gap: var(--spacing-sm);
    margin-bottom: var(--spacing-md);
    font-size: var(--font-size-sm);
}

.stars {
    color: var(--secondary-color);
    letter-spacing: 2px;
}

.rating-count {
    color: var(--text-light);
}

.product-footer {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-top: var(--spacing-md);
    border-top: 1px solid var(--border-color);
    margin-top: auto;
}

.product-price {
    font-size: 1.25rem;
    font-weight: 700;
    color: var(--secondary-color);
}

.view-all {
    display: flex;
    justify-content: center;
}

/* ===== BENEFITS SECTION (Flexbox) ===== */
.benefits {
    padding: var(--spacing-2xl) 0;
    background: var(--primary-color);
    color: var(--bg-white);
}

.benefits-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: var(--spacing-xl);
}

.benefit-card {
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    padding: var(--spacing-lg);
}

.benefit-icon {
    font-size: 3rem;
    margin-bottom: var(--spacing-md);
}

.benefit-card h3 {
    font-size: var(--font-size-lg);
    font-weight: 600;
    margin-bottom: var(--spacing-sm);
}

.benefit-card p {
    font-size: var(--font-size-sm);
    opacity: 0.9;
    font-weight: 300;
}

/* ===== ABOUT SECTION (Flexbox) ===== */
.about {
    padding: var(--spacing-2xl) 0;
    background: var(--bg-white);
}

.about-content {
    display: flex;
    align-items: center;
    gap: var(--spacing-2xl);
}

.about-text {
    flex: 1;
    min-width: 300px;
}

.about-text p {
    color: var(--text-light);
    margin-bottom: var(--spacing-lg);
    line-height: 1.8;
    font-weight: 300;
    font-size: var(--font-size-lg);
}

.about-stats {
    display: flex;
    justify-content: space-around;
    margin-top: var(--spacing-xl);
    padding-top: var(--spacing-xl);
    border-top: 1px solid var(--border-color);
}

.stat {
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    gap: var(--spacing-sm);
}

.stat-number {
    font-family: var(--font-display);
    font-size: 2rem;
    font-weight: 700;
    color: var(--secondary-color);
}

.stat-label {
    font-size: var(--font-size-sm);
    color: var(--text-light);
}

.about-visual {
    flex: 1;
    min-width: 300px;
}

.about-image {
    width: 100%;
    aspect-ratio: 1;
    border-radius: var(--radius-lg);
    background: linear-gradient(45deg, #d4af37, #f4d03f);
    box-shadow: var(--shadow-lg);
}

/* ===== NEWSLETTER SECTION ===== */
.newsletter {
    padding: var(--spacing-2xl) 0;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    color: var(--bg-white);
}

.newsletter-content {
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    gap: var(--spacing-lg);
}

.newsletter-content h2 {
    font-family: var(--font-display);
    font-size: var(--font-size-2xl);
    font-weight: 700;
}

.newsletter-form {
    display: flex;
    width: 100%;
    max-width: 500px;
    gap: var(--spacing-sm);
}

.newsletter-form input {
    flex: 1;
    padding: 0.75rem 1.25rem;
    border: none;
    border-radius: var(--radius-md);
    font-family: inherit;
    font-size: var(--font-size-base);
}

.newsletter-form input::placeholder {
    color: #999;
}

.newsletter-form .btn {
    white-space: nowrap;
}

.newsletter-disclaimer {
    font-size: var(--font-size-sm);
    opacity: 0.9;
    font-weight: 300;
}

/* ===== FOOTER (Flexbox) ===== */
.footer {
    background: var(--primary-color);
    color: var(--bg-white);
    padding: var(--spacing-2xl) 0 var(--spacing-lg);
}

.footer-content {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: var(--spacing-2xl);
    margin-bottom: var(--spacing-2xl);
    padding-bottom: var(--spacing-2xl);
    border-bottom: 1px solid rgba(255, 255, 255, 0.1);
}

.footer-section h4 {
    font-family: var(--font-display);
    font-size: 1.1rem;
    font-weight: 600;
    margin-bottom: var(--spacing-md);
    color: var(--secondary-color);
}

.footer-section p {
    font-size: var(--font-size-sm);
    line-height: 1.8;
    opacity: 0.9;
    margin-bottom: var(--spacing-md);
}

.footer-section ul {
    list-style: none;
    display: flex;
    flex-direction: column;
    gap: var(--spacing-sm);
}

.footer-section a {
    font-size: var(--font-size-sm);
    opacity: 0.8;
    transition: var(--transition-fast);
}

.footer-section a:hover {
    opacity: 1;
    color: var(--secondary-color);
}

.social-links {
    display: flex;
    gap: var(--spacing-md);
}

.footer-bottom {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: var(--spacing-lg);
    font-size: var(--font-size-sm);
}

.footer-left {
    opacity: 0.8;
}

.footer-links {
    display: flex;
    gap: var(--spacing-lg);
}

.footer-links a {
    transition: var(--transition-fast);
}

.footer-links a:hover {
    color: var(--secondary-color);
}

/* ===== TOAST NOTIFICATION ===== */
.toast {
    position: fixed;
    bottom: var(--spacing-lg);
    right: var(--spacing-lg);
    background: var(--primary-color);
    color: var(--bg-white);
    padding: var(--spacing-md) var(--spacing-lg);
    border-radius: var(--radius-md);
    box-shadow: var(--shadow-lg);
    z-index: 2000;
    opacity: 0;
    transform: translateY(20px);
    transition: all 0.3s ease;
    pointer-events: none;
}

.toast.show {
    opacity: 1;
    transform: translateY(0);
    pointer-events: auto;
}

/* ===== ANIMATIONS ===== */
@keyframes slideInLeft {
    from {
        opacity: 0;
        transform: translateX(-50px);
    }
    to {
        opacity: 1;
        transform: translateX(0);
    }
}

@keyframes slideInRight {
    from {
        opacity: 0;
        transform: translateX(50px);
    }
    to {
        opacity: 1;
        transform: translateX(0);
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

/* ===== RESPONSIVE DESIGN (Mobile First) ===== */

/* Tablets (768px and up) */
@media (max-width: 768px) {
    :root {
        --font-size-3xl: 2rem;
        --font-size-2xl: 1.5rem;
        --spacing-2xl: 2.5rem;
    }

    /* Navigation */
    .navbar-container {
        padding: 0 var(--spacing-md);
    }

    .logo-text {
        font-size: 1.25rem;
    }

    .menu-toggle {
        display: flex;
    }

    .nav-menu {
        position: absolute;
        top: 100%;
        left: 0;
        right: 0;
        background: var(--bg-white);
        flex-direction: column;
        gap: 0;
        padding: var(--spacing-lg);
        border-bottom: 1px solid var(--border-color);
        max-height: 0;
        overflow: hidden;
        transition: max-height 0.3s ease;
    }

    .nav-menu.active {
        max-height: 400px;
    }

    .nav-link {
        padding: var(--spacing-md) 0;
        display: block;
    }

    .nav-cta {
        flex-direction: column;
        width: 100%;
    }

    /* Hero Section */
    .hero-container {
        flex-direction: column;
        padding: var(--spacing-lg);
        gap: var(--spacing-lg);
    }

    .hero-title {
        font-size: 1.75rem;
    }

    /* Products Grid */
    .products-grid {
        grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
        gap: var(--spacing-lg);
    }

    /* About Section */
    .about-content {
        flex-direction: column;
        gap: var(--spacing-lg);
    }

    .about-stats {
        flex-direction: column;
        gap: var(--spacing-lg);
    }

    /* Newsletter Form */
    .newsletter-form {
        flex-direction: column;
    }

    /* Footer */
    .footer-bottom {
        flex-direction: column;
        text-align: center;
    }
}

/* Mobile (480px and below) */
@media (max-width: 480px) {
    :root {
        --spacing-lg: 1.5rem;
        --spacing-xl: 2rem;
        --font-size-2xl: 1.25rem;
        --font-size-3xl: 1.5rem;
    }

    .container {
        padding: 0 var(--spacing-md);
    }

    /* Navigation */
    .navbar-container {
        padding: 0 var(--spacing-md);
    }

    .logo-text {
        font-size: 1rem;
        letter-spacing: 1px;
    }

    .nav-cta {
        order: -1;
    }

    /* Hero */
    .hero-title {
        font-size: 1.5rem;
    }

    .hero-subtitle {
        font-size: 1rem;
    }

    /* Products */
    .products-grid {
        grid-template-columns: 1fr;
    }

    .section-title {
        font-size: 1.5rem;
    }

    /* Footer */
    .footer-content {
        grid-template-columns: 1fr;
        gap: var(--spacing-lg);
    }

    .footer-links {
        flex-direction: column;
        gap: var(--spacing-sm);
    }

    /* Toast */
    .toast {
        left: var(--spacing-md);
        right: var(--spacing-md);
        bottom: var(--spacing-md);
    }
}

/* ===== ACCESSIBILITY ===== */
@media (prefers-reduced-motion: reduce) {
    * {
        animation-duration: 0.01ms !important;
        animation-iteration-count: 1 !important;
        transition-duration: 0.01ms !important;
    }
}

/* Focus visible styles for keyboard navigation */
button:focus-visible,
a:focus-visible,
input:focus-visible {
    outline: 2px solid var(--secondary-color);
    outline-offset: 2px;
}

/* Dark mode support (optional) */
@media (prefers-color-scheme: dark) {
    :root {
        --bg-white: #1a1a1a;
        --bg-light: #2a2a2a;
        --text-dark: #e8e8e8;
        --text-light: #b0b0b0;
        --border-color: #333333;
    }

    .hero {
        background: linear-gradient(135deg, #2a2a2a 0%, #1a1a1a 100%);
    }
}
```


## OUTPUT
<img width="1913" height="1029" alt="Screenshot 2026-05-05 183611" src="https://github.com/user-attachments/assets/80058276-3843-479e-b613-0338f8cfe15c" />

<img width="1910" height="1027" alt="Screenshot 2026-05-05 183636" src="https://github.com/user-attachments/assets/73207290-e204-4dc7-b004-001f69383dcf" />

<img width="1913" height="1026" alt="Screenshot 2026-05-05 183714" src="https://github.com/user-attachments/assets/a5542580-3670-4524-967a-5b4a958647ed" />



## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
