# mariapetkovska
Maria's website
[index.html.html](https://github.com/user-attachments/files/22100410/index.html.html)
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Expert Copywriting & Content Strategy | Convert More Customers</title>
    <meta name="description" content="Professional copywriting and content strategy services for marketing agencies and eCommerce businesses. Increase conversions, boost engagement, and grow revenue with strategic copy.">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        :root {
            --primary-color: #0077b5;
            --secondary-color: #00a0dc;
            --accent-color: #ff6b6b;
            --success-color: #28a745;
            --dark-color: #2c3e50;
            --light-gray: #f8f9fa;
            --medium-gray: #6c757d;
            --white: #ffffff;
        }
        
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
            line-height: 1.6;
            color: var(--dark-color);
            scroll-behavior: smooth;
        }
        
        /* Header */
        .header {
            position: fixed;
            top: 0;
            width: 100%;
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            box-shadow: 0 2px 20px rgba(0, 0, 0, 0.1);
            z-index: 1000;
            transition: all 0.3s ease;
        }
        
        .nav {
            max-width: 1200px;
            margin: 0 auto;
            padding: 1rem 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--primary-color);
            text-decoration: none;
        }
        
        .nav-links {
            display: flex;
            list-style: none;
            gap: 2rem;
        }
        
        .nav-links a {
            text-decoration: none;
            color: var(--dark-color);
            font-weight: 500;
            transition: color 0.3s ease;
        }
        
        .nav-links a:hover {
            color: var(--primary-color);
        }
        
        .cta-button {
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            color: var(--white);
            padding: 0.75rem 1.5rem;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(0, 119, 181, 0.3);
        }
        
        .cta-button:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 25px rgba(0, 119, 181, 0.4);
        }
        
        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: var(--white);
            padding: 120px 0 80px;
            text-align: center;
            position: relative;
            overflow: hidden;
        }
        
        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1000 1000"><polygon fill="rgba(255,255,255,0.1)" points="0,1000 1000,0 1000,1000"/></svg>');
            background-size: cover;
        }
        
        .hero-content {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 2rem;
            position: relative;
            z-index: 1;
        }
        
        .hero h1 {
            font-size: clamp(2.5rem, 5vw, 4rem);
            font-weight: 700;
            margin-bottom: 1.5rem;
            line-height: 1.2;
        }
        
        .hero .subtitle {
            font-size: clamp(1.2rem, 2.5vw, 1.5rem);
            margin-bottom: 2rem;
            opacity: 0.9;
        }
        
        .hero-cta {
            display: flex;
            gap: 1rem;
            justify-content: center;
            flex-wrap: wrap;
            margin-top: 2rem;
        }
        
        .btn-primary {
            background: var(--accent-color);
            color: var(--white);
            padding: 1rem 2rem;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            font-size: 1.1rem;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(255, 107, 107, 0.3);
        }
        
        .btn-primary:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 25px rgba(255, 107, 107, 0.4);
        }
        
        .btn-secondary {
            background: rgba(255, 255, 255, 0.2);
            color: var(--white);
            padding: 1rem 2rem;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            font-size: 1.1rem;
            transition: all 0.3s ease;
            backdrop-filter: blur(10px);
            border: 2px solid rgba(255, 255, 255, 0.3);
        }
        
        .btn-secondary:hover {
            background: rgba(255, 255, 255, 0.3);
            transform: translateY(-2px);
        }
        
        /* Results Section */
        .results {
            padding: 80px 0;
            background: var(--light-gray);
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 2rem;
        }
        
        .results-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 3rem;
            margin-top: 3rem;
        }
        
        .result-card {
            background: var(--white);
            padding: 2rem;
            border-radius: 15px;
            text-align: center;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease;
        }
        
        .result-card:hover {
            transform: translateY(-5px);
        }
        
        .result-number {
            font-size: 3rem;
            font-weight: 700;
            color: var(--primary-color);
            margin-bottom: 0.5rem;
        }
        
        .result-text {
            font-size: 1.1rem;
            color: var(--medium-gray);
        }
        
        /* Services Section */
        .services {
            padding: 80px 0;
            background: var(--white);
        }
        
        .section-header {
            text-align: center;
            margin-bottom: 4rem;
        }
        
        .section-title {
            font-size: clamp(2rem, 4vw, 3rem);
            font-weight: 700;
            color: var(--dark-color);
            margin-bottom: 1rem;
        }
        
        .section-subtitle {
            font-size: 1.2rem;
            color: var(--medium-gray);
            max-width: 600px;
            margin: 0 auto;
        }
        
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }
        
        .service-card {
            background: var(--white);
            padding: 2.5rem;
            border-radius: 20px;
            box-shadow: 0 10px 40px rgba(0, 0, 0, 0.1);
            transition: all 0.3s ease;
            border-top: 4px solid var(--primary-color);
        }
        
        .service-card:nth-child(2) {
            border-top-color: var(--accent-color);
        }
        
        .service-card:nth-child(3) {
            border-top-color: var(--success-color);
        }
        
        .service-card:nth-child(4) {
            border-top-color: var(--secondary-color);
        }
        
        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.15);
        }
        
        .service-icon {
            font-size: 3rem;
            margin-bottom: 1.5rem;
        }
        
        .service-title {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--dark-color);
            margin-bottom: 1rem;
        }
        
        .service-description {
            color: var(--medium-gray);
            margin-bottom: 1.5rem;
            line-height: 1.6;
        }
        
        .service-benefits {
            list-style: none;
            margin-bottom: 2rem;
        }
        
        .service-benefits li {
            padding: 0.5rem 0;
            position: relative;
            padding-left: 1.5rem;
        }
        
        .service-benefits li::before {
            content: "✓";
            position: absolute;
            left: 0;
            color: var(--success-color);
            font-weight: bold;
        }
        
        /* Process Section */
        .process {
            padding: 80px 0;
            background: var(--light-gray);
        }
        
        .process-steps {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin-top: 3rem;
        }
        
        .process-step {
            background: var(--white);
            padding: 2rem;
            border-radius: 15px;
            text-align: center;
            position: relative;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.1);
        }
        
        .step-number {
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            color: var(--white);
            width: 50px;
            height: 50px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: 700;
            font-size: 1.2rem;
            margin: 0 auto 1.5rem;
        }
        
        .step-title {
            font-size: 1.3rem;
            font-weight: 700;
            margin-bottom: 1rem;
            color: var(--dark-color);
        }
        
        .step-description {
            color: var(--medium-gray);
        }
        
        /* Testimonials */
        .testimonials {
            padding: 80px 0;
            background: var(--white);
        }
        
        .testimonial-card {
            background: var(--light-gray);
            padding: 2.5rem;
            border-radius: 20px;
            margin: 2rem 0;
            position: relative;
        }
        
        .testimonial-text {
            font-size: 1.2rem;
            font-style: italic;
            margin-bottom: 1.5rem;
            line-height: 1.6;
        }
        
        .testimonial-author {
            font-weight: 600;
            color: var(--primary-color);
        }
        
        /* CTA Section */
        .final-cta {
            padding: 80px 0;
            background: linear-gradient(135deg, var(--dark-color), #34495e);
            color: var(--white);
            text-align: center;
        }
        
        .cta-content h2 {
            font-size: clamp(2rem, 4vw, 3rem);
            margin-bottom: 1rem;
        }
        
        .cta-content p {
            font-size: 1.2rem;
            margin-bottom: 2rem;
            opacity: 0.9;
        }
        
        /* Footer */
        .footer {
            background: var(--dark-color);
            color: var(--white);
            padding: 40px 0;
            text-align: center;
        }
        
        .footer p {
            opacity: 0.8;
        }
        
        /* Mobile Menu */
        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            font-size: 1.5rem;
            color: var(--dark-color);
            cursor: pointer;
        }
        
        /* Responsive Design */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }
            
            .mobile-menu-btn {
                display: block;
            }
            
            .hero-cta {
                flex-direction: column;
                align-items: center;
            }
            
            .btn-primary, .btn-secondary {
                width: 100%;
                max-width: 300px;
                text-align: center;
            }
            
            .results-grid {
                grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
                gap: 2rem;
            }
            
            .services-grid {
                grid-template-columns: 1fr;
            }
            
            .process-steps {
                grid-template-columns: 1fr;
            }
        }
        
        /* Animations */
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        .fade-in-up {
            animation: fadeInUp 0.6s ease forwards;
        }
        
        /* Scroll animations */
        .animate-on-scroll {
            opacity: 0;
            transform: translateY(30px);
            transition: all 0.6s ease;
        }
        
        .animate-on-scroll.animated {
            opacity: 1;
            transform: translateY(0);
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header class="header">
        <nav class="nav">
            <a href="#" class="logo">CopyStrategist</a>
            <ul class="nav-links">
                <li><a href="#services">Services</a></li>
                <li><a href="#process">Process</a></li>
                <li><a href="#results">Results</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
            <a href="#contact" class="cta-button">Get Started</a>
            <button class="mobile-menu-btn">☰</button>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="hero-content">
            <h1 class="fade-in-up">Turn Your Traffic Into Revenue With Copy That Converts</h1>
            <p class="subtitle fade-in-up">I help marketing agencies and eCommerce businesses boost conversions by 25-50% with strategic copywriting and content that actually sells.</p>
            <div class="hero-cta fade-in-up">
                <a href="#contact" class="btn-primary">Get Your Copy Audit</a>
                <a href="#services" class="btn-secondary">See My Services</a>
            </div>
        </div>
    </section>

    <!-- Results Section -->
    <section class="results">
        <div class="container">
            <div class="section-header animate-on-scroll">
                <h2 class="section-title">Results That Speak For Themselves</h2>
                <p class="section-subtitle">Real outcomes from real clients who trusted me with their copy</p>
            </div>
            <div class="results-grid">
                <div class="result-card animate-on-scroll">
                    <div class="result-number">45%</div>
                    <div class="result-text">Average conversion rate increase</div>
                </div>
                <div class="result-card animate-on-scroll">
                    <div class="result-number">$2.3M</div>
                    <div class="result-text">Additional revenue generated for clients</div>
                </div>
                <div class="result-card animate-on-scroll">
                    <div class="result-number">180%</div>
                    <div class="result-text">Improvement in email open rates</div>
                </div>
                <div class="result-card animate-on-scroll">
                    <div class="result-number">60%</div>
                    <div class="result-text">Reduction in customer acquisition costs</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section class="services" id="services">
        <div class="container">
            <div class="section-header animate-on-scroll">
                <h2 class="section-title">Services That Drive Results</h2>
                <p class="section-subtitle">Comprehensive copywriting and content strategy solutions for growing businesses</p>
            </div>
            <div class="services-grid">
                <div class="service-card animate-on-scroll">
                    <div class="service-icon">📧</div>
                    <h3 class="service-title">Email Copywriting</h3>
                    <p class="service-description">Transform your email campaigns from inbox clutter to revenue generators with psychology-driven copy that builds relationships and drives sales.</p>
                    <ul class="service-benefits">
                        <li>Welcome sequence optimization</li>
                        <li>Promotional campaign copy</li>
                        <li>Subject line psychology</li>
                        <li>List segmentation strategy</li>
                        <li>A/B testing frameworks</li>
                    </ul>
                </div>
                <div class="service-card animate-on-scroll">
                    <div class="service-icon">🌐</div>
                    <h3 class="service-title">Website Copywriting</h3>
                    <p class="service-description">Convert more visitors with homepage and landing page copy that speaks directly to your customers' needs and guides them to take action.</p>
                    <ul class="service-benefits">
                        <li>Homepage conversion optimization</li>
                        <li>Landing page copy</li>
                        <li>Product page descriptions</li>
                        <li>About page storytelling</li>
                        <li>CTA optimization</li>
                    </ul>
                </div>
                <div class="service-card animate-on-scroll">
                    <div class="service-icon">✍️</div>
                    <h3 class="service-title">Blog Writing</h3>
                    <p class="service-description">Attract and convert your ideal customers with strategic blog content that positions you as the authority and generates qualified leads.</p>
                    <ul class="service-benefits">
                        <li>SEO-optimized blog posts</li>
                        <li>Thought leadership articles</li>
                        <li>Case study creation</li>
                        <li>Guest posting</li>
                        <li>Content series planning</li>
                    </ul>
                </div>
                <div class="service-card animate-on-scroll">
                    <div class="service-icon">🎯</div>
                    <h3 class="service-title">Content Strategy</h3>
                    <p class="service-description">Get a complete roadmap for content that actually drives business results, with systems and frameworks you can scale.</p>
                    <ul class="service-benefits">
                        <li>Content audit & analysis</li>
                        <li>Strategic content planning</li>
                        <li>Brand voice development</li>
                        <li>Content calendar creation</li>
                        <li>ROI measurement frameworks</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Process Section -->
    <section class="process" id="process">
        <div class="container">
            <div class="section-header animate-on-scroll">
                <h2 class="section-title">My Proven Process</h2>
                <p class="section-subtitle">How I turn your content challenges into revenue opportunities</p>
            </div>
            <div class="process-steps">
                <div class="process-step animate-on-scroll">
                    <div class="step-number">1</div>
                    <h3 class="step-title">Discovery & Research</h3>
                    <p class="step-description">I dive deep into your business, audience, and competitors to understand what really drives your customers to buy.</p>
                </div>
                <div class="process-step animate-on-scroll">
                    <div class="step-number">2</div>
                    <h3 class="step-title">Strategy Development</h3>
                    <p class="step-description">Based on research insights, I create a custom content strategy designed to hit your specific business goals.</p>
                </div>
                <div class="process-step animate-on-scroll">
                    <div class="step-number">3</div>
                    <h3 class="step-title">Copy Creation</h3>
                    <p class="step-description">I write conversion-focused copy that speaks your customers' language and guides them toward taking action.</p>
                </div>
                <div class="process-step animate-on-scroll">
                    <div class="step-number">4</div>
                    <h3 class="step-title">Test & Optimize</h3>
                    <p class="step-description">We track performance, run tests, and continuously optimize to maximize your ROI and long-term results.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials -->
    <section class="testimonials" id="results">
        <div class="container">
            <div class="section-header animate-on-scroll">
                <h2 class="section-title">What Clients Say</h2>
                <p class="section-subtitle">Real feedback from agencies and eCommerce businesses I've helped grow</p>
            </div>
            <div class="testimonial-card animate-on-scroll">
                <p class="testimonial-text">"Working with [Your Name] completely transformed our email marketing. Our welcome series conversion rate jumped from 12% to 23% in just 60 days. The ROI has been incredible."</p>
                <div class="testimonial-author">- Sarah M., eCommerce Beauty Brand</div>
            </div>
            <div class="testimonial-card animate-on-scroll">
                <p class="testimonial-text">"Finally found a copywriter who understands agency life. The website copy they delivered helped us attract higher-value clients and positioned us as the premium choice in our market."</p>
                <div class="testimonial-author">- Mike R., Digital Marketing Agency</div>
            </div>
        </div>
    </section>

    <!-- Final CTA -->
    <section class="final-cta" id="contact">
        <div class="container">
            <div class="cta-content animate-on-scroll">
                <h2>Ready to Transform Your Copy Into Revenue?</h2>
                <p>Let's discuss how strategic copywriting can help you attract better clients, increase conversions, and grow your business.</p>
                <a href="mailto:hello@yourname.com" class="btn-primary">Get Your Free Strategy Call</a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="footer">
        <div class="container">
            <p>&copy; 2025 CopyStrategist. All rights reserved. | Professional copywriting and content strategy services</p>
        </div>
    </footer>

    <script>
        // Scroll animations
        const animateOnScroll = () => {
            const elements = document.querySelectorAll('.animate-on-scroll');
            elements.forEach(element => {
                const elementTop = element.getBoundingClientRect().top;
                const elementVisible = 150;
                
                if (elementTop < window.innerHeight - elementVisible) {
                    element.classList.add('animated');
                }
            });
        }

        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // Initialize animations
        window.addEventListener('scroll', animateOnScroll);
        window.addEventListener('load', animateOnScroll);

        // Header background on scroll
        window.addEventListener('scroll', () => {
            const header = document.querySelector('.header');
            if (window.scrollY > 50) {
                header.style.background = 'rgba(255, 255, 255, 0.98)';
            } else {
                header.style.background = 'rgba(255, 255, 255, 0.95)';
            }
        });
    </script>
</body>
</html>
