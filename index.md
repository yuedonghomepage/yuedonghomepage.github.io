---
layout: default
title: Yue Dong - Personal Homepage
---

<section id="home">
    <div class="container">
        <div class="profile-grid">
            <div class="profile-img">
                <img src="assets/images/photo2.jpg" alt="Yue Dong">
            </div>
            <div class="profile-info">
                <h1>Yue Dong (董悦)</h1>
                <p class="role">Principal Researcher</p>
                <p class="affiliation">Spatial Intelligence Group, Microsoft Research Asia</p>
                <div class="bio">
                    <p>I am a principal researcher at Spatial Intelligence Group in Microsoft Research Asia. My work focuses mainly on appearance modeling, neural rendering and 3D vision.</p>
                </div>
                <div class="contact-info">
                    <p><strong>Email:</strong> yuedong [at] microsoft.com</p>
                </div>
            </div>
        </div>
    </div>
</section>

<section id="publications">
    <div class="container">
        <h2>Publications</h2>
        <div class="publication-list">
            {% for paper in site.data.publications %}
            <article class="publication-item">
                <div class="pub-thumb">
                    <a href="{{ paper.links[0].url }}">
                        <img src="{{ paper.thumbnail }}" alt="{{ paper.title }} Teaser" loading="lazy">
                    </a>
                </div>
                <div class="pub-content">
                    <h3><a href="{{ paper.links[0].url }}">{{ paper.title }}</a></h3>
                    <div class="authors">{{ paper.authors }}</div>
                    <div class="venue">{{ paper.venue }}</div>
                    <div class="links">
                        {% for link in paper.links %}
                        <a href="{{ link.url }}">{{ link.name }}</a>
                        {% endfor %}
                    </div>
                </div>
            </article>
            {% endfor %}
        </div>
    </div>
</section>

<section id="activities">
    <div class="container">
        <h2>Professional Activities</h2>
        <div class="content-block">
            <h3>Paper Committees</h3>
            <p>SIGGRAPH 2024</p>
            <p>SIGGRAPH Asia 2022</p>
            <p>Pacific Graphics 2015, 2016, 2019, 2022, 2023</p>
            <p>Eurographics 2019, 2021</p>
            <p>Eurographics Symposium on Rendering 2020, 2021, 2026</p>
            <p>ACM Symposium on Virtual Reality Software and Technology 2021</p>
            <p>SIGGRAPH Asia Posters and Tech Comms 2019, 2020</p>
            <p>CAD Graphics 2015, 2016, 2017, 2019, 2021</p>

            <h3 style="margin-top: 1.5rem;">Journal Editor</h3>
            <p>IEEE TVCG Associate Editor</p>

            <h3 style="margin-top: 1.5rem;">Reviewer</h3>
            <p>ACM SIGGRAPH, ACM SIGGRAPH Asia, Eurographics, Pacific Graphics, CGI</p>
            <p>ACM TOG, IEEE TVCG, The Visual Computer, Computer Graphics Forum, Computers and Graphics</p>
        </div>
    </div>
</section>
