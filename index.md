---
layout: default
title: Welcome to My Site
---

<link rel="stylesheet" href="{{ '/assets/css/styles.css' | relative_url }}">

<div class="container">
    <!-- Menu -->
    <ul class="menu">
        <li><a href="/">Home</a></li>
        <li><a href="/about/">About</a></li>
        <li><a href="/blog/">Blog</a></li>
        <!-- Add additional menu items as needed -->
    </ul>

    <div class="welcome-section">
        <h1>Welcome to My Jekyll Site</h1>
        <p>Hello, and welcome to my Jekyll-powered website! Here, I share my thoughts, ideas, and experiences on various topics.</p>
    </div>

    <!-- Latest Video Section -->
    <div class="video-section">
        <h2>Watch My Latest Video</h2>
        <div class="video-wrapper">
            <iframe width="560" height="315" src="https://www.youtube.com/embed/CBD2Bjj4XRk" frameborder="0" allowfullscreen></iframe>
        </div>
    </div>

    <!-- Latest Blog Posts Section -->
    <div class="latest-posts">
        <h2>Latest Blog Posts</h2>
        <div class="post-list">
            {% for post in site.posts limit: 3 %}
            <div class="post">
                <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
                <p>{{ post.excerpt | strip_html | truncate: 150 }}</p>
            </div>
            {% endfor %}
        </div>
    </div>

    <!-- About Me Section -->
    <div class="about-section">
        <h2>About Me</h2>
        <p>I'm [Your Name], a passionate [your profession/hobby/interest]. I love [mention what you love about your profession/hobby/interest]. Feel free to explore my site and get to know me better!</p>
    </div>

    <!-- Connect with Me Section -->
    <div class="connect-section">
        <h2>Connect with Me</h2>
        <div class="social-links">
            <a href="https://github.com/your-username">GitHub</a>
            <a href="https://twitter.com/your-twitter">Twitter</a>
            <a href="https://linkedin.com/in/your-linkedin">LinkedIn</a>
        </div>
    </div>
</div>
