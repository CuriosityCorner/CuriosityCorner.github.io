---
layout: home
title: Welcome to My Jekyll Site
---

<style>
/* Custom CSS for background images */
.welcome-section {
    background-image: url('/assets/welcome-background.jpg');
    background-size: cover;
    background-position: center;
    color: white;
    padding: 100px 0; /* Adjust padding as needed */
}

.about-section {
    background-image: url('/assets/about-background.jpg');
    background-size: cover;
    background-position: center;
    color: white;
    padding: 100px 0; /* Adjust padding as needed */
}
</style>

# Welcome to My Jekyll Site

<div class="welcome-section">
    <!-- Content of the welcome section -->
    Hello, and welcome to my Jekyll-powered website! Here, I share my thoughts, ideas, and experiences on various topics.
</div>

## Latest Blog Posts

{% for post in site.posts %}
### [{{ post.title }}]({{ post.url }})
{{ post.excerpt | strip_html | truncatewords: 25 }}
- Published on {{ post.date | date: "%B %d, %Y" }}
{% endfor %}

<div class="about-section">
    <!-- Content of the about section -->
    ## About Me
    
    I'm [Your Name], a passionate [your profession/hobby/interest]. I love [mention what you love about your profession/hobby/interest]. Feel free to explore my site and get to know me better!
</div>

## Connect with Me

- [GitHub](https://github.com/your-username)
- [Twitter](https://twitter.com/your-twitter)
- [LinkedIn](https://linkedin.com/in/your-linkedin)

Feel free to reach out and connect with me on social media!

