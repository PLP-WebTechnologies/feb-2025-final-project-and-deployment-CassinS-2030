# Final Project and Deployment

## Objectives
Build a fully functional web application.
Apply HTML, CSS, and JavaScript concepts learned.
Deploy the project using GitHub Pages, Netlify, or Vercel.

## Instructions
Choose one of the following project ideas:
Blog Website: Implement a multi-page site with navigation.
Ecommerce Website: Implement a multi-page site with navigation.

>[!NOTE]
> - Include at least:
> - A responsive design.
> - JavaScript interactivity.
> - A deployment link.

## Tasks

Create a well-structured HTML5 document.
Use at least 5 different HTML elements.
Ensure semantic correctness.

Good luck and happy coding! 🚀💻





/blog-website/
│── index.html
│── about.html
│── contact.html
│── styles.css
│── script.js
│── images/



index.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Blog</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <div class="container">
            <h1>My Blog</h1>
            <nav>
                <ul>
                    <li><a href="index.html" class="active">Home</a></li>
                    <li><a href="about.html">About</a></li>
                    <li><a href="contact.html">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <main class="container">
        <section class="featured-post">
            <article>
                <h2>Featured Post</h2>
                <img src="images/featured.jpg" alt="Featured post image">
                <p>This is the excerpt of the featured blog post. Click to read more...</p>
                <button class="read-more">Read More</button>
            </article>
        </section>

        <section class="blog-posts">
            <h2>Recent Posts</h2>
            <div class="posts-grid" id="postsContainer">
                <!-- Posts will be loaded here via JavaScript -->
            </div>
        </section>
    </main>

    <aside class="newsletter">
        <div class="container">
            <h3>Subscribe to our Newsletter</h3>
            <form id="newsletterForm">
                <input type="email" placeholder="Your email address" required>
                <button type="submit">Subscribe</button>
            </form>
        </div>
    </aside>

    <footer>
        <div class="container">
            <p>&copy; 2023 My Blog. All rights reserved.</p>
        </div>
    </footer>

    <script src="script.js"></script>
</body>
</html>

about.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>About - My Blog</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <div class="container">
            <h1>My Blog</h1>
            <nav>
                <ul>
                    <li><a href="index.html">Home</a></li>
                    <li><a href="about.html" class="active">About</a></li>
                    <li><a href="contact.html">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <main class="container">
        <section class="about-content">
            <h2>About Us</h2>
            <p>Welcome to My Blog, a place where we share thoughts, ideas, and stories about technology, travel, and lifestyle.</p>
            <p>Our mission is to create meaningful content that inspires and informs our readers.</p>
            <div class="team">
                <h3>Our Team</h3>
                <div class="team-members">
                    <div class="member">
                        <img src="images/team1.jpg" alt="Team member 1">
                        <h4>Jane Doe</h4>
                        <p>Founder & Editor</p>
                    </div>
                    <div class="member">
                        <img src="images/team2.jpg" alt="Team member 2">
                        <h4>John Smith</h4>
                        <p>Content Writer</p>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <footer>
        <div class="container">
            <p>&copy; 2023 My Blog. All rights reserved.</p>
        </div>
    </footer>
</body>
</html>


contact.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact - My Blog</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <div class="container">
            <h1>My Blog</h1>
            <nav>
                <ul>
                    <li><a href="index.html">Home</a></li>
                    <li><a href="about.html">About</a></li>
                    <li><a href="contact.html" class="active">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <main class="container">
        <section class="contact-form">
            <h2>Contact Us</h2>
            <form id="contactForm">
                <div class="form-group">
                    <label for="name">Name:</label>
                    <input type="text" id="name" required>
                </div>
                <div class="form-group">
                    <label for="email">Email:</label>
                    <input type="email" id="email" required>
                </div>
                <div class="form-group">
                    <label for="message">Message:</label>
                    <textarea id="message" rows="5" required></textarea>
                </div>
                <button type="submit">Send Message</button>
            </form>
        </section>

        <section class="contact-info">
            <h3>Other Ways to Reach Us</h3>
            <p>Email: contact@myblog.com</p>
            <p>Phone: (123) 456-7890</p>
            <div class="social-media">
                <a href="#">Twitter</a>
                <a href="#">Facebook</a>
                <a href="#">Instagram</a>
            </div>
        </section>
    </main>

    <footer>
        <div class="container">
            <p>&copy; 2023 My Blog. All rights reserved.</p>
        </div>
    </footer>

    <script src="script.js"></script>
</body>
</html>


style.css
/* Global Styles */
:root {
    --primary-color: #3498db;
    --secondary-color: #2c3e50;
    --light-color: #ecf0f1;
    --dark-color: #2c3e50;
    --success-color: #2ecc71;
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    line-height: 1.6;
    color: #333;
    background-color: #f9f9f9;
}

.container {
    width: 90%;
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

/* Header Styles */
header {
    background-color: var(--secondary-color);
    color: white;
    padding: 1rem 0;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}

header h1 {
    margin-bottom: 1rem;
}

nav ul {
    display: flex;
    list-style: none;
}

nav ul li {
    margin-right: 1.5rem;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-weight: 500;
    transition: color 0.3s;
}

nav ul li a:hover {
    color: var(--primary-color);
}

nav ul li a.active {
    color: var(--primary-color);
    border-bottom: 2px solid var(--primary-color);
}

/* Main Content Styles */
main {
    padding: 2rem 0;
}

.featured-post {
    margin-bottom: 3rem;
}

.featured-post article {
    background: white;
    border-radius: 8px;
    overflow: hidden;
    box-shadow: 0 3px 10px rgba(0, 0, 0, 0.1);
}

.featured-post img {
    width: 100%;
    height: 300px;
    object-fit: cover;
}

.featured-post h2 {
    padding: 1rem;
    font-size: 1.8rem;
    color: var(--dark-color);
}

.featured-post p {
    padding: 0 1rem 1rem;
    color: #666;
}

.read-more {
    display: inline-block;
    background: var(--primary-color);
    color: white;
    padding: 0.5rem 1rem;
    margin: 0 1rem 1rem;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    transition: background 0.3s;
}

.read-more:hover {
    background: #2980b9;
}

.blog-posts h2 {
    margin-bottom: 1.5rem;
    font-size: 1.5rem;
    color: var(--dark-color);
}

.posts-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
    gap: 1.5rem;
}

.post-card {
    background: white;
    border-radius: 8px;
    overflow: hidden;
    box-shadow: 0 3px 10px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s;
}

.post-card:hover {
    transform: translateY(-5px);
}

.post-card img {
    width: 100%;
    height: 200px;
    object-fit: cover;
}

.post-content {
    padding: 1rem;
}

.post-content h3 {
    margin-bottom: 0.5rem;
    color: var(--dark-color);
}

.post-content p {
    color: #666;
    margin-bottom: 1rem;
}

.post-meta {
    display: flex;
    justify-content: space-between;
    color: #888;
    font-size: 0.9rem;
}

/* About Page Styles */
.about-content {
    background: white;
    padding: 2rem;
    border-radius: 8px;
    box-shadow: 0 3px 10px rgba(0, 0, 0, 0.1);
}

.about-content h2 {
    margin-bottom: 1rem;
    color: var(--dark-color);
}

.about-content p {
    margin-bottom: 1rem;
}

.team {
    margin-top: 2rem;
}

.team h3 {
    margin-bottom: 1.5rem;
    color: var(--dark-color);
}

.team-members {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
    gap: 2rem;
}

.member {
    text-align: center;
}

.member img {
    width: 150px;
    height: 150px;
    border-radius: 50%;
    object-fit: cover;
    margin-bottom: 1rem;
    border: 3px solid var(--primary-color);
}

.member h4 {
    color: var(--dark-color);
    margin-bottom: 0.5rem;
}

/* Contact Page Styles */
.contact-form {
    background: white;
    padding: 2rem;
    border-radius: 8px;
    box-shadow: 0 3px 10px rgba(0, 0, 0, 0.1);
    margin-bottom: 2rem;
}

.contact-form h2 {
    margin-bottom: 1.5rem;
    color: var(--dark-color);
}

.form-group {
    margin-bottom: 1.5rem;
}

.form-group label {
    display: block;
    margin-bottom: 0.5rem;
    font-weight: 500;
    color: var(--dark-color);
}

.form-group input,
.form-group textarea {
    width: 100%;
    padding: 0.75rem;
    border: 1px solid #ddd;
    border-radius: 4px;
    font-family: inherit;
}

.form-group textarea {
    resize: vertical;
}

.contact-form button {
    background: var(--primary-color);
    color: white;
    padding: 0.75rem 1.5rem;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    font-size: 1rem;
    transition: background 0.3s;
}

.contact-form button:hover {
    background: #2980b9;
}

.contact-info {
    background: white;
    padding: 2rem;
    border-radius: 8px;
    box-shadow: 0 3px 10px rgba(0, 0, 0, 0.1);
}

.contact-info h3 {
    margin-bottom: 1rem;
    color: var(--dark-color);
}

.contact-info p {
    margin-bottom: 1rem;
}

.social-media {
    margin-top: 1.5rem;
}

.social-media a {
    display: inline-block;
    margin-right: 1rem;
    color: var(--primary-color);
    text-decoration: none;
    font-weight: 500;
}

.social-media a:hover {
    text-decoration: underline;
}

/* Newsletter Styles */
.newsletter {
    background: var(--secondary-color);
    color: white;
    padding: 2rem 0;
    text-align: center;
}

.newsletter h3 {
    margin-bottom: 1rem;
}

.newsletter input {
    padding: 0.75rem;
    width: 300px;
    max-width: 100%;
    border: none;
    border-radius: 4px 0 0 4px;
}

.newsletter button {
    padding: 0.75rem 1.5rem;
    background: var(--primary-color);
    color: white;
    border: none;
    border-radius: 0 4px 4px 0;
    cursor: pointer;
    transition: background 0.3s;
}

.newsletter button:hover {
    background: #2980b9;
}

/* Footer Styles */
footer {
    background: var(--dark-color);
    color: white;
    text-align: center;
    padding: 1.5rem 0;
    margin-top: 2rem;
}

/* Responsive Styles */
@media (max-width: 768px) {
    nav ul {
        flex-direction: column;
    }

    nav ul li {
        margin-right: 0;
        margin-bottom: 0.5rem;
    }

    .featured-post img {
        height: 200px;
    }

    .newsletter form {
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    .newsletter input {
        border-radius: 4px;
        margin-bottom: 0.5rem;
    }

    .newsletter button {
        border-radius: 4px;
        width: 300px;
        max-width: 100%;
    }
}

@media (max-width: 480px) {
    .container {
        width: 100%;
        padding: 0 15px;
    }

    .featured-post img {
        height: 150px;
    }
}



script.js
// Sample blog posts data
const blogPosts = [
    {
        id: 1,
        title: "Getting Started with JavaScript",
        excerpt: "Learn the basics of JavaScript and start your journey as a web developer.",
        image: "images/post1.jpg",
        date: "May 15, 2023",
        category: "Programming"
    },
    {
        id: 2,
        title: "Responsive Design Principles",
        excerpt: "Understand the core principles of creating websites that work on all devices.",
        image: "images/post2.jpg",
        date: "May 10, 2023",
        category: "Design"
    },
    {
        id: 3,
        title: "The Future of Web Development",
        excerpt: "Exploring emerging trends and technologies in the web development landscape.",
        image: "images/post3.jpg",
        date: "May 5, 2023",
        category: "Technology"
    },
    {
        id: 4,
        title: "CSS Grid vs Flexbox",
        excerpt: "When to use each layout system for optimal results in your projects.",
        image: "images/post4.jpg",
        date: "April 28, 2023",
        category: "CSS"
    },
    {
        id: 5,
        title: "Building Your First API",
        excerpt: "A step-by-step guide to creating your first RESTful API with Node.js.",
        image: "images/post5.jpg",
        date: "April 20, 2023",
        category: "Backend"
    }
];

// DOM Content Loaded
document.addEventListener('DOMContentLoaded', function() {
    // Load blog posts
    if (document.getElementById('postsContainer')) {
        loadBlogPosts();
    }

    // Newsletter form submission
    const newsletterForm = document.getElementById('newsletterForm');
    if (newsletterForm) {
        newsletterForm.addEventListener('submit', handleNewsletterSubmit);
    }

    // Contact form submission
    const contactForm = document.getElementById('contactForm');
    if (contactForm) {
        contactForm.addEventListener('submit', handleContactSubmit);
    }

    // Read more button functionality
    const readMoreBtn = document.querySelector('.read-more');
    if (readMoreBtn) {
        readMoreBtn.addEventListener('click', function() {
            alert('This would normally redirect to the full blog post page.');
        });
    }
});

// Function to load blog posts
function loadBlogPosts() {
    const postsContainer = document.getElementById('postsContainer');
    
    blogPosts.forEach(post => {
        const postCard = document.createElement('div');
        postCard.className = 'post-card';
        
        postCard.innerHTML = `
            <img src="${post.image}" alt="${post.title}">
            <div class="post-content">
                <h3>${post.title}</h3>
                <p>${post.excerpt}</p>
                <div class="post-meta">
                    <span>${post.category}</span>
                    <span>${post.date}</span>
                </div>
            </div>
        `;
        
        postCard.addEventListener('click', function() {
            alert(`This would normally redirect to the full post: ${post.title}`);
        });
        
        postsContainer.appendChild(postCard);
    });
}

// Newsletter form handler
function handleNewsletterSubmit(e) {
    e.preventDefault();
    const email = e.target.querySelector('input').value;
    
    // In a real app, you would send this to a server
    console.log(`Subscribed email: ${email}`);
    alert('Thank you for subscribing to our newsletter!');
    e.target.reset();
}

// Contact form handler
function handleContactSubmit(e) {
    e.preventDefault();
    const name = document.getElementById('name').value;
    const email = document.getElementById('email').value;
    const message = document.getElementById('message').value;
    
    // In a real app, you would send this to a server
    console.log(`Contact form submitted:
    Name: ${name}
    Email: ${email}
    Message: ${message}`);
    
    alert('Thank you for your message! We will get back to you soon.');
    e.target.reset();
}



