---
title: Documentations
---
# Documentations as Code for AIOps

Landing page.

CSS utility classes come in handy when you to want to override default styles to create additional whitespace (margins/padding), correct unexpected shifts in font size or weight, add color, or hide (or show) something at a specific screen size.

This is a test of Github PR.

<div class="section-index">
    <hr class="panel-line">
    {% for post in site.docs  %}
        <!-- list the "index.md" title of your documents below if you want it to be displayed in the Documentations landing page -->
        {% if 
        post.title == "Random Document for Demo" or
        post.title == "TELUS SD-WAN Services Generic DSD" %}        
            <div class="entry">
            <h5><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h5>
            <p>{{ post.description }}</p>
            </div>
        {% endif %}
    {% endfor %}
</div>