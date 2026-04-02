<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lumina Bistro | Modern Dining</title>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        /* CSS STYLES */
        :root {
            --gold: #c5a059;
            --dark: #121212;
            --light: #f4f4f4;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Poppins', sans-serif;
            background-color: var(--light);
            color: var(--dark);
            line-height: 1.6;
        }

        header {
            height: 100vh;
            background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)), 
                        url('https://images.unsplash.com/photo-1514362545857-3bc16c4c7d1b?ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80');
            background-size: cover;
            background-position: center;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            color: white;
            padding: 20px;
        }

        nav {
            position: fixed;
            top: 0;
            width: 100%;
            padding: 20px 50px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            background: rgba(0,0,0,0.8);
            z-index: 1000;
        }

        .logo {
            font-family: 'Playfair Display', serif;
            font-size: 24px;
            color: var(--gold);
        }

        .nav-links {
            display: flex;
            list-style: none;
        }

        .nav-links li {
            margin-left: 20px;
        }

        .nav-links a {
            text-decoration: none;
            color: white;
            font-size: 14px;
            text-transform: uppercase;
            letter-spacing: 1px;
            transition: 0.3s;
        }

        .nav-links a:hover {
            color: var(--gold);
        }

        h1 {
            font-family: 'Playfair Display', serif;
            font-size: 4rem;
            margin-bottom: 10px;
        }

        .btn {
            margin-top: 20px;
            padding: 12px 30px;
            background: var(--gold);
            color: white;
            text-decoration: none;
            border-radius: 5px;
            text-transform: uppercase;
            font-weight: bold;
            transition: 0.3s;
        }

        .btn:hover {
            background: #a38245;
        }

        section {
            padding: 80px 10%;
        }

        .section-title {
            text-align: center;
            font-family: 'Playfair Display', serif;
            font-size: 2.5rem;
            margin-bottom: 40px;
        }

        /* Menu Grid */
        .menu-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .menu-item {
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            transition: 0.3s;
        }

        .menu-item:hover {
            transform: translateY(-5px);
        }

        .menu-item h3 {
            display: flex;
            justify-content: space-between;
            border-bottom: 1px solid #ddd;
            padding-bottom: 10px;
            margin-bottom: 10px;
        }

        .price {
            color: var(--gold);
        }

        /* Footer */
        footer {
            background: var(--dark);
            color: white;
            text-align: center;
            padding: 50px;
        }

        .contact-info {
            margin-bottom: 20px;
        }

        @media (max-width: 768px) {
            h1 { font-size: 2.5rem; }
            nav { padding: 20px; }
            .nav-links { display: none; }
        }
    </style>
</head>
<body>

    <nav>
        <div class="logo">LUMINA BISTRO</div>
        <ul class="nav-links">
            <li><a href="#home">Home</a></li>
            <li><a href="#menu">Menu</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <header id="home">
        <h1>Experience Modern Dining</h1>
        <p>Fresh ingredients, bold flavors, unforgettable nights.</p>
        <a href="#menu" class="btn">View Menu</a>
    </header>

    <section id="menu">
        <h2 class="section-title">Our Menu</h2>
        <div class="menu-grid">
            <div class="menu-item">
                <h3><span>Truffle Gnocchi</span> <span class="price">$24</span></h3>
                <p>Handmade potato gnocchi, black truffle cream, and aged parmesan.</p>
            </div>
            <div class="menu-item">
                <h3><span>Seared Scallops</span> <span class="price">$28</span></h3>
                <p>Pan-seared scallops with cauliflower purée and lemon butter.</p>
            </div>
            <div class="menu-item">
                <h3><span>Dry-Aged Steak</span> <span class="price">$42</span></h3>
                <p>12oz Ribeye served with rosemary butter and roasted roots.</p>
            </div>
            <div class="menu-item">
                <h3><span>Honey Glazed Salmon</span> <span class="price">$29</span></h3>
                <p>Wild-caught salmon with ginger-honey glaze and bok choy.</p>
            </div>
            <div class="menu-item">
                <h3><span>Wild Mushroom Risotto</span> <span class="price">$22</span></h3>
                <p>Arborio rice, seasonal forest mushrooms, and truffle oil.</p>
            </div>
            <div class="menu-item">
                <h3><span>Dark Chocolate Fondant</span> <span class="price">$12</span></h3>
                <p>Warm lava cake with Madagascar vanilla bean gelato.</p>
            </div>
        </div>
    </section>

    <section id="contact" style="background-color: #eee;">
        <h2 class="section-title">Visit Us</h2>
        <div style="text-align: center; max-width: 600px; margin: 0 auto;">
            <p><strong>Address:</strong> 123 Culinary Ave, Foodie City, FC 54321</p>
            <p><strong>Phone:</strong> (555) 123-4567</p>
            <p><strong>Hours:</strong> Tue-Sun: 5pm - 11pm</p>
            <br>
            <a href="tel:5551234567" class="btn">Call for Reservation</a>
        </div>
    </section>

    <footer>
        <p>&copy; 2023 Lumina Bistro. 100% Free Website Template.</p>
    </footer>

</body>
</html>
