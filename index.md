---
layout: home
title: Welcome to My Jekyll Site
---

<style>
/* Custom CSS for improved styling */
.container {
    max-width: 800px;
    margin: 0 auto;
    padding: 20px;
}

.welcome-section {
    text-align: center;
    margin-bottom: 50px;
}

.latest-posts {
    margin-bottom: 50px;
}

.about-section {
    background-color: #f5f5f5;
    padding: 50px;
    border-radius: 5px;
    text-align: center;
}

.connect-section {
    text-align: center;
    margin-top: 50px;
}

.connect-section a {
    display: inline-block;
    margin-right: 10px;
    margin-bottom: 10px;
    padding: 10px 20px;
    background-color: #007bff;
    color: #ffffff;
    text-decoration: none;
    border-radius: 5px;
}

.connect-section a:hover {
    background-color: #0056b3;
}
</style>

<div class="container">
    <div class="welcome-section">
        <h1>Welcome to My Jekyll Site</h1>
        <p>Hello, and welcome to my Jekyll-powered website! Here, I share my thoughts, ideas, and experiences on various topics.</p>
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
        <p>I'm [Your Name], a passionate [your profession/hobby/interest]. I love [mention what you love about your profession/hobby/interest]. Feel free to explore my site and get to know me better!</p>
    </div>

    <div class="connect-section">
        <h2>Connect with Me</h2>
        <a href="https://github.com/your-username">GitHub</a>
        <a href="https://twitter.com/your-twitter">Twitter</a>
        <a href="https://linkedin.com/in/your-linkedin">LinkedIn</a>
    </div>
</div>
