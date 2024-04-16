---
layout: home
title: Welcome to Curiosity Corner
---

<style>
/* Custom CSS for improved styling */
body {
    font-family: 'Roboto', sans-serif; /* Use Google Fonts */
    color: #333;
    background-color: #f9f9f9;
    margin: 0;
    padding: 0;
}

.container {
    max-width: 800px;
    margin: 0 auto;
    padding: 20px;
}

/* Add menu styles */
.menu {
    list-style-type: none;
    margin: 0;
    padding: 0;
    text-align: center;
}

.menu li {
    display: inline;
    margin-right: 20px;
}

.menu li:last-child {
    margin-right: 0;
}

.menu a {
    text-decoration: none;
    color: #555;
    font-weight: bold;
    font-size: 18px;
    transition: color 0.3s ease-in-out; /* Add smooth color transition */
}

.menu a:hover {
    color: #007bff; /* Change color on hover */
}

/* Style headings */
h1, h2, h3 {
    color: #333;
    font-weight: bold;
}

/* Style paragraphs */
p {
    color: #555;
    line-height: 1.6;
}

/* Style links */
a {
    color: #007bff;
    text-decoration: none;
}

a:hover {
    color: #0056b3;
}
</style>

<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">

<div class="container">
    <!-- Menu -->
    <ul class="menu">
        <li><a href="/">Home</a></li>
        <li><a href="/about/">About</a></li>
        <li><a href="/blog/">Blog</a></li>
        <!-- Add additional menu items as needed -->
    </ul>

    <div class="welcome-section">
        <h1>About us</h1>
        <p> Here we bring you latest new and updates</p>
    </div>
    
   <div class="video-section">
        <h2>Watch My Latest Video</h2>
        <!-- Embed YouTube video -->
        <iframe width="560" height="315" src="https://www.youtube.com/embed/CBD2Bjj4XRk" frameborder="0" allowfullscreen></iframe>
    </div>
    
    <div class="latest-posts">
        <h2>Latest Blog Posts</h2>
        {% for post in site.posts limit: 3 %}
        <div>
            <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
            <p>{{ post.excerpt | strip_html | truncate: 150 }}</p>
        </div>
        {% endfor %}
    </div>

    <div class="about-section">
        <h2>About Me</h2>
        <p>I'm a passionate chef/blogger. I love dancing. Feel free to explore my site and get to know me better!</p>
    </div>

    <div class="connect-section">
        <h2>Connect with Me</h2>
        <a href="https://github.com/your-username">GitHub</a>
        <a href="https://twitter.com/your-twitter">Twitter</a>
        <a href="https://linkedin.com/in/your-linkedin">LinkedIn</a>
    </div>
</div>
