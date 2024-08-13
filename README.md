# Responsive-landing-page
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Home Page</title>
    <link rel="stylesheet" href="responsive.css">
</head>
<body>
    <header>
        <div class="container">
            <h1>🌟 Responsive Landing page 🌟</h1>
            <nav>
                <a href="#home">🏠 Home</a>
                <a href="#about">💡 About</a>
                <a href="#services">🔧 Services</a>
                <a href="#contact">📞 Contact</a>
            </nav>
        </div>
    </header>

    <main>
        <div class="hero">
            <div class="container">
                <h2>Your Journey Begins Here 🌍</h2>
                <p>Discover amazing content and explore our offerings. We’re glad you’re here!</p>
                <a href="#services" class="cta-button">Explore Services 🚀</a>
            </div>
        </div>

        <section id="about">
            <div class="container">
                <h2>About Us 💼</h2>
                <p>We are a dedicated team committed to providing the best services and creating an impact.</p>
            </div>
        </section>

        <section id="services">
            <div class="container">
                <h2>Our Services 🛠️</h2>
                <div class="service">
                    <h3>Web Development</h3>
                    <p>Custom websites and web applications to meet your needs.</p>
                </div>
                <div class="service">
                    <h3>Graphic Design</h3>
                    <p>Eye-catching designs to make your brand stand out.</p>
                </div>
                <div class="service">
                    <h3>SEO Optimization</h3>
                    <p>Improve your website's visibility and ranking on search engines.</p>
                </div>
            </div>
        </section>

        <section id="contact">
            <div class="container">
                <h2>Contact Us 📧</h2>
                <p>We’d love to hear from you! Reach out to us through email or follow us on social media.</p>
            </div>
        </section>
    </main>

    <footer>
        <div class="container">
            <p>&copy; 2024 My Awesome Website. All rights reserved. 🌐</p>
        </div>
    </footer>

    <script src="responsive.js"></script>
</body>
</html>

#external css

/* General Styles */
body, html {
    margin: 0;
    padding: 0;
    font-family: 'Arial', sans-serif;
    scroll-behavior: smooth;
    background-color: #510416;
    color: #f3dede;
}

/* Scrollbar Styles */
body::-webkit-scrollbar {
    width: 12px;
}

body::-webkit-scrollbar-track {
    background: #220505;
}

body::-webkit-scrollbar-thumb {
    background-color: #000000;
    border-radius: 10px;
    border: 3px solid #2d1d1d;
}

/* Container Styles */
.container {
    width: 90%;
    max-width: 1200px;
    margin: 0 auto;
    padding: 10px;
}

/* Header Styles */
header {
    background: linear-gradient(135deg, #000000, #debbd7);
    color: #f4ecef;
    padding: 20px 0;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    margin-bottom: 30px;
    position: sticky;
    top: 0;
    z-index: 1000;
    transition: background-color 0.3s ease;
}

header.scrolled {
    background-color: #debbd7;
}

header .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

header h1 {
    margin: 0;
    font-size: 28px;
    text-transform: uppercase;
    transition: color 0.3s ease;
}

nav {
    display: flex;
    gap: 10px;
}

nav a {
    color: #240b18;
    text-decoration: none;
    padding: 10px 20px;
    border-radius: 30px;
    background-color: #ff9a8b;
    transition: background-color 0.3s ease, transform 0.3s ease;
    font-weight: bold;
}

nav a:hover {
    background-color: #ff6f61;
    transform: scale(1.1);
}

nav a.active {
    background-color: #2e2827;
    color: #fff;
}

/* Hero Section */
.hero {
    background: linear-gradient(135deg, #f9a825, #ff5722);
    color: #fff;
    padding: 80px 0;
    text-align: center;
    margin-bottom: 30px;
    position: relative;
    overflow: hidden;
    border-radius: 15px;
}

.hero h2 {
    font-size: 48px;
    margin: 0;
    animation: fadeIn 2s ease-in-out;
}

.hero p {
    font-size: 24px;
    margin: 20px 0;
    animation: fadeIn 2.5s ease-in-out;
}

.cta-button {
    display: inline-block;
    padding: 15px 40px;
    background-color: #fff;
    color: #ff5722;
    border-radius: 25px;
    text-decoration: none;
    font-size: 20px;
    font-weight: bold;
    transition: background-color 0.3s ease, color 0.3s ease, transform 0.3s ease;
}

.cta-button:hover {
    background-color: #ff5722;
    color: #fff;
    transform: translateY(-5px);
}

.hero::after {
    content: "";
    background: url('path-to-your-background-image.jpg') center/cover no-repeat;
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    opacity: 0.1;
    z-index: -1;
}

/* Animations */
@keyframes fadeIn {
    0% { opacity: 0; transform: translateY(-20px); }
    100% { opacity: 1; transform: translateY(0); }
}

/* Main Content Area */
section {
    background-color: #ffffff;
    padding: 40px 20px;
    margin-bottom: 30px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    border-radius: 15px;
    transition: transform 0.3s ease;
}

section:hover {
    transform: translateY(-10px);
}

section h2 {
    margin-top: 0;
    font-size: 32px;
    color: #2e0804;
    text-align: center;
    margin-bottom: 20px;
}

section p {
    margin-bottom: 0;
    line-height: 1.8;
    font-size: 18px;
    color: #555;
}

/* Services Section */
.service {
    padding: 20px;
    border: 1px solid #0f0936;
    border-radius: 15px;
    margin-bottom: 20px;
    transition: background-color 0.3s ease, transform 0.3s ease;
}

.service:hover {
    background-color: #e8320e;
    color: #260f0f;
    transform: translateY(-5px);
}

.service h3 {
    margin-top: 0;
    font-size: 24px;
    color: #200c3d; 
}

/* Footer Styles */
footer {
    background-color: #333333;
    color: #ffffff;
    padding: 20px 0;
    text-align: center;
    border-radius: 15px;
    margin-top: 30px;
}

footer p {
    margin: 0;
    font-size: 16px;
}

/* Responsive Styles */
@media (max-width: 768px) {
    header .container {
        flex-direction: column;
        align-items: center;
    }

    nav {
        flex-direction: column;
        gap: 15px;
    }

    nav a {
        width: 100%;
        text-align: center;
    }

    main .container {
        padding: 0 20px;
    }

    .hero h2 {
        font-size: 36px;
    }

    .hero p {
        font-size: 18px;
    }

    .cta-button {
        padding: 12px 30px;
        font-size: 16px;
    }

    section h2 {
        font-size: 28px;
    }

    section p {
        font-size: 16px;
    }
}
#java script


// JavaScript for smooth scrolling and active link highlighting
document.addEventListener('DOMContentLoaded', () => {
    const navLinks = document.querySelectorAll('nav a');

    navLinks.forEach(anchor => {
        anchor.addEventListener('click', function(e) {
            e.preventDefault();
            const targetSection = document.querySelector(this.getAttribute('href'));
            
            if (targetSection) {
                targetSection.scrollIntoView({
                    behavior: 'smooth'
                });
            }
        });
    });

    // Highlight the active link as the user scrolls
    const sections = document.querySelectorAll('section');
    const options = {
        threshold: 0.6
    };

    const observer = new IntersectionObserver((entries, observer) => {
        entries.forEach(entry => {
            if (entry.isIntersecting) {
                navLinks.forEach(link => {
                    link.classList.remove('active');
                    if (link.getAttribute('href').substring(1) === entry.target.id) {
                        link.classList.add('active');
                    }
                });
            }
        });
    }, options);

    sections.forEach(section => {
        observer.observe(section);
    });
});


