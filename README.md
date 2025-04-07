# krak-app
AI crypto trading bot and advanced analytics tracking for beginners and experienced crypto traders.
/* Kraken Trading Bot Web App Styles */

/* Variables */
:root {
    /* Kraken brand colors */
    --primary-color: #5741d9;
    --secondary-color: #4a3ab3;
    --accent-color: #8c79f7;
    --dark-color: #1c1c28;
    --light-color: #f5f5f7;
    --success-color: #00c853;
    --warning-color: #ffc107;
    --danger-color: #f44336;
    --info-color: #2196f3;
    
    /* Typography */
    --font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    --heading-font-weight: 700;
    --body-font-size: 16px;
    
    /* Spacing */
    --spacing-xs: 0.25rem;
    --spacing-sm: 0.5rem;
    --spacing-md: 1rem;
    --spacing-lg: 1.5rem;
    --spacing-xl: 2rem;
    --spacing-xxl: 3rem;
    
    /* Border radius */
    --border-radius-sm: 4px;
    --border-radius-md: 8px;
    --border-radius-lg: 16px;
    --border-radius-xl: 24px;
    
    /* Shadows */
    --shadow-sm: 0 1px 3px rgba(0, 0, 0, 0.12), 0 1px 2px rgba(0, 0, 0, 0.24);
    --shadow-md: 0 4px 6px rgba(0, 0, 0, 0.1), 0 1px 3px rgba(0, 0, 0, 0.08);
    --shadow-lg: 0 10px 20px rgba(0, 0, 0, 0.1), 0 3px 6px rgba(0, 0, 0, 0.05);
    --shadow-xl: 0 15px 25px rgba(0, 0, 0, 0.15), 0 5px 10px rgba(0, 0, 0, 0.05);
    
    /* Transitions */
    --transition-fast: 0.2s ease;
    --transition-normal: 0.3s ease;
    --transition-slow: 0.5s ease;
}

/* Reset and Base Styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    font-size: var(--body-font-size);
    scroll-behavior: smooth;
}

body {
    font-family: var(--font-family);
    line-height: 1.6;
    color: var(--dark-color);
    background-color: var(--light-color);
    min-height: 100vh;
    display: flex;
    flex-direction: column;
}

h1, h2, h3, h4, h5, h6 {
    font-weight: var(--heading-font-weight);
    line-height: 1.2;
    margin-bottom: var(--spacing-md);
    color: var(--dark-color);
}

h1 {
    font-size: 2.5rem;
}

h2 {
    font-size: 2rem;
}

h3 {
    font-size: 1.5rem;
}

p {
    margin-bottom: var(--spacing-md);
}

a {
    color: var(--primary-color);
    text-decoration: none;
    transition: color var(--transition-fast);
}

a:hover {
    color: var(--secondary-color);
}

ul {
    list-style-type: none;
}

img {
    max-width: 100%;
    height: auto;
}

/* Container */
.container {
    width: 100%;
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 var(--spacing-md);
}

/* Buttons */
.btn {
    display: inline-block;
    padding: var(--spacing-sm) var(--spacing-lg);
    border-radius: var(--border-radius-md);
    font-weight: 600;
    text-align: center;
    cursor: pointer;
    transition: all var(--transition-fast);
    border: none;
    font-size: 1rem;
}

.btn-primary {
    background-color: var(--primary-color);
    color: white;
}

.btn-primary:hover {
    background-color: var(--secondary-color);
    color: white;
}

.btn-outline {
    background-color: transparent;
    color: var(--primary-color);
    border: 2px solid var(--primary-color);
}

.btn-outline:hover {
    background-color: var(--primary-color);
    color: white;
}

.btn-large {
    padding: var(--spacing-md) var(--spacing-xl);
    font-size: 1.1rem;
}

.btn-sm {
    padding: var(--spacing-xs) var(--spacing-sm);
    font-size: 0.9rem;
}

.btn-full {
    width: 100%;
}

.btn:disabled {
    opacity: 0.7;
    cursor: not-allowed;
}

/* Navigation */
.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: var(--spacing-md) var(--spacing-xl);
    background-color: white;
    box-shadow: var(--shadow-sm);
    position: sticky;
    top: 0;
    z-index: 100;
}

.logo {
    display: flex;
    align-items: center;
}

.logo img {
    height: 40px;
    margin-right: var(--spacing-sm);
}

.logo span {
    font-size: 1.2rem;
    font-weight: 700;
    color: var(--primary-color);
}

.nav-links {
    display: flex;
    gap: var(--spacing-lg);
}

.nav-links a {
    color: var(--dark-color);
    font-weight: 500;
    position: relative;
}

.nav-links a:hover {
    color: var(--primary-color);
}

.nav-links a.active {
    color: var(--primary-color);
}

.nav-links a.active::after {
    content: '';
    position: absolute;
    bottom: -5px;
    left: 0;
    width: 100%;
    height: 2px;
    background-color: var(--primary-color);
}

.auth-buttons {
    display: flex;
    gap: var(--spacing-md);
}

.menu-toggle {
    display: none;
    font-size: 1.5rem;
    cursor: pointer;
}

/* Hero Section */
.hero {
    display: flex;
    align-items: center;
    padding: var(--spacing-xxl) var(--spacing-xl);
    background: linear-gradient(135deg, #f5f7ff 0%, #e3e6ff 100%);
}

.hero-content {
    flex: 1;
    padding-right: var(--spacing-xl);
}

.hero-content h1 {
    font-size: 3rem;
    margin-bottom: var(--spacing-md);
    color: var(--dark-color);
}

.hero-content p {
    font-size: 1.2rem;
    margin-bottom: var(--spacing-lg);
    color: #666;
}

.hero-buttons {
    display: flex;
    gap: var(--spacing-md);
}

.hero-image {
    flex: 1;
    display: flex;
    justify-content: center;
    align-items: center;
}

.hero-image img {
    max-width: 100%;
    border-radius: var(--border-radius-lg);
    box-shadow: var(--shadow-lg);
}

/* Features Preview */
.features-preview {
    padding: var(--spacing-xxl) var(--spacing-xl);
    text-align: center;
    background-color: white;
}

.features-preview h2 {
    margin-bottom: var(--spacing-xl);
}

.features-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: var(--spacing-lg);
}

.feature-card {
    padding: var(--spacing-lg);
    border-radius: var(--border-radius-md);
    box-shadow: var(--shadow-md);
    transition: transform var(--transition-normal);
}

.feature-card:hover {
    transform: translateY(-5px);
}

.feature-card i {
    font-size: 2.5rem;
    color: var(--primary-color);
    margin-bottom: var(--spacing-md);
}

.feature-card h3 {
    margin-bottom: var(--spacing-sm);
}

/* Pricing Preview */
.pricing-preview {
    padding: var(--spacing-xxl) var(--spacing-xl);
    text-align: center;
    background-color: var(--light-color);
}

.pricing-preview h2 {
    margin-bottom: var(--spacing-xl);
}

.pricing-cards {
    display: flex;
    justify-content: center;
    gap: var(--spacing-lg);
    margin-bottom: var(--spacing-lg);
    flex-wrap: wrap;
}

.pricing-card {
    background-color: white;
    border-radius: var(--border-radius-lg);
    box-shadow: var(--shadow-md);
    overflow: hidden;
    width: 300px;
    transition: transform var(--transition-normal);
    position: relative;
}

.pricing-card:hover {
    transform: translateY(-5px);
    box-shadow: var(--shadow-lg);
}

.pricing-card.popular {
    transform: scale(1.05);
    border: 2px solid var(--primary-color);
}

.pricing-card.popular:hover {
    transform: scale(1.05) translateY(-5px);
}

.popular-badge {
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    background-color: var(--primary-color);
    color: white;
    padding: var(--spacing-xs) 0;
    text-align: center;
    font-weight: 600;
    font-size: 0.9rem;
}

.pricing-header {
    padding: var(--spacing-lg);
    text-align: center;
    border-bottom: 1px solid #eee;
}

.pricing-header h3 {
    margin-bottom: var(--spacing-sm);
}

.price {
    font-size: 2rem;
    font-weight: 700;
    color: var(--primary-color);
}

.price span {
    font-size: 1rem;
    color: #666;
}

.pricing-features {
    padding: var(--spacing-lg);
}

.pricing-features ul {
    margin-bottom: var(--spacing-lg);
    text-align: left;
}

.pricing-features li {
    margin-bottom: var(--spacing-sm);
    display: flex;
    align-items: center;
}

.pricing-features li i {
    color: var(--success-color);
    margin-right: var(--spacing-sm);
}

.pricing-note {
    font-size: 0.9rem;
    color: #666;
}

/* Testimonials */
.testimonials {
    padding: var(--spacing-xxl) var(--spacing-xl);
    text-align: center;
    background-color: white;
}

.testimonials h2 {
    margin-bottom: var(--spacing-xl);
}

.testimonial-slider {
    max-width: 800px;
    margin: 0 auto;
    position: relative;
}

.testimonial {
    padding: var(--spacing-lg);
    margin-bottom: var(--spacing-lg);
}

.testimonial-content {
    background-color: var(--light-color);
    padding: var(--spacing-lg);
    border-radius: var(--border-radius-md);
    margin-bottom: var(--spacing-lg);
    position: relative;
    box-shadow: var(--shadow-sm);
}

.testimonial-content::after {
    content: '';
    position: absolute;
    bottom: -10px;
    left: 50%;
    transform: translateX(-50%);
    width: 0;
    height: 0;
    border-left: 10px solid transparent;
    border-right: 10px solid transparent;
    border-top: 10px solid var(--light-color);
}

.testimonial-content p {
    font-style: italic;
    margin-bottom: 0;
}

.testimonial-author {
    display: flex;
    align-items: center;
    justify-content: center;
}

.testimonial-author img {
    width: 60px;
    height: 60px;
    border-radius: 50%;
    margin-right: var(--spacing-md);
    object-fit: cover;
}

.testimonial-author h4 {
    margin-bottom: 0;
}

.testimonial-author p {
    margin-bottom: 0;
    color: #666;
    font-size: 0.9rem;
}

.testimonial-dots {
    display: flex;
    justify-content: center;
    gap: var(--spacing-sm);
}

.dot {
    width: 10px;
    height: 10px;
    border-radius: 50%;
    background-color: #ccc;
    cursor: pointer;
    transition: background-color var(--transition-fast);
}

.dot.active {
    background-color: var(--primary-color);
}

/* Modal */
.modal {
    display: none;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.5);
    z-index: 1000;
    justify-content: center;
    align-items: center;
}

.modal.active {
    display: flex;
}

.modal-content {
    background-color: white;
    padding: var(--spacing-xl);
    border-radius: var(--border-radius-lg);
    box-shadow: var(--shadow-lg);
    max-width: 500px;
    width: 90%;
    position: relative;
}

.close-modal {
    position: absolute;
    top: var(--spacing-md);
    right: var(--spacing-md);
    font-size: 1.5rem;
    cursor: pointer;
    color: #666;
}

.close-modal:hover {
    color: var(--danger-color);
}

/* Forms */
.form-group {
    margin-bottom: var(--spacing-md);
}

.form-group label {
    display: block;
    margin-bottom: var(--spacing-xs);
    font-weight: 500;
}

.form-group input {
    width: 100%;
    padding: var(--spacing-sm);
    border: 1px solid #ddd;
    border-radius: var(--border-radius-sm);
    font-size: 1rem;
}

.form-group input:focus {
    outline: none;
    border-color: var(--primary-color);
}

.form-footer {
    text-align: center;
    margin-top: var(--spacing-md);
    font-size: 0.9rem;
}

/* Welcome Modal */
.welcome-content {
    text-align: center;
}

.success-icon {
    font-size: 4rem;
    color: var(--success-color);
    margin-bottom: var(--spacing-md);
}

/* Footer */
footer {
    background-color: var(--dark-color);
    color: white;
    padding-top: var(--spacing-xl);
    margin-top: auto;
}

.footer-content {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: var(--spacing-xl);
    padding: 0 var(--spacing-xl) var(--spacing-xl);
}

.footer-section h3 {
    color: white;
    margin-bottom: var(--spacing-md);
    position: relative;
    padding-bottom: var(--spacing-sm);
}

.footer-section h3::after {
    content: '';
    position: absolute;
    bottom: 0;
    left: 0;
    width: 50px;
    height: 2px;
    background-color: var(--primary-color);
}

.footer-section p {
    margin-bottom: var(--spacing-sm);
}

.footer-section ul li {
    margin-bottom: var(--spacing-xs);
}

.footer-section ul li a {
    color: #ccc;
    transition: color var(--transition-fast);
}

.footer-section ul li a:hover {
    color: white;
}

.social-links {
    display: flex;
    gap: var(--spacing-sm);
    margin-top: var(--spacing-md);
}

.social-links a {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 40px;
    height: 40px;
    border-radius: 50%;
    background-color: rgba(255, 255, 255, 0.1);
    color: white;
    transition: background-color var(--transition-fast);
}

.social-links a:hover {
    background-color: var(--primary-color);
}

.footer-bottom {
    text-align: center;
    padding: var(--spacing-md) 0;
    border-top: 1px solid rgba(255, 255, 255, 0.1);
}

/* Utility Classes */
.hidden {
    display: none !important;
}

.text-center {
    text-align: center;
}

.mt-1 { margin-top: var(--spacing-sm); }
.mt-2 { margin-top: var(--spacing-md); }
.mt-3 { margin-top: var(--spacing-lg); }
.mt-4 { margin-top: var(--spacing-xl); }
.mt-5 { margin-top: var(--spacing-xxl); }

.mb-1 { margin-bottom: var(--spacing-sm); }
.mb-2 { margin-bottom: var(--spacing-md); }
.mb-3 { margin-bottom: var(--spacing-lg); }
.mb-4 { margin-bottom: var(--spacing-xl); }
.mb-5 { margin-bottom: var(--spacing-xxl); }

/* Responsive Styles */
@media (max-width: 992px) {
    .hero {
        flex-direction: column;
        text-align: center;
    }
    
    .hero-content {
        padding-right: 0;
        margin-bottom: var(--spacing-xl);
    }
    
    .hero-buttons {
        justify-content: center;
    }
    
    .pricing-cards {
        flex-direction: column;
        align-items: center;
    }
    
    .pricing-card {
        width: 100%;
        max-width: 350px;
        margin-bottom: var(--spacing-lg);
    }
    
    .pricing-card.popular {
        transform: scale(1);
    }
    
    .pricing-card.popular:hover {
        transform: translateY(-5px);
    }
}

@media (max-width: 768px) {
    .nav-links, .auth-buttons {
        display: none;
    }
    
    .menu-toggle {
        display: block;
    }
    
    .nav-links.active {
        display: flex;
        flex-direction: column;
        position: absolute;
        top: 70px;
        left: 0;
        right: 0;
        background-color: white;
        padding: var(--spacing-md);
        box-shadow: var(--shadow-md);
    }
    
    .auth-buttons.active {
        display: flex;
        flex-direction: column;
        gap: var(--spacing-sm);
        padding: var(--spacing-md);
        background-color: white;
        position: absolute;
        top: 200px;
        left: 0;
        right: 0;
        box-shadow: var(--shadow-md);
    }
    
    .features-grid {
        grid-template-columns: 1fr;
    }
}

@media (max-width: 576px) {
    h1 {
        font-size: 2rem;
    }
    
    h2 {
        font-size: 1.5rem;
    }
    
    .hero-content h1 {
        font-size: 2.2rem;
    }
    
    .hero-buttons {
        flex-direction: column;
        gap: var(--spacing-sm);
    }
    
    .footer-content {
        grid-template-columns: 1fr;
    }
}
