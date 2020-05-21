---
layout: default
title: Research
---

<html lang="en">

<body>

 <!-- ======= Research Section ======= -->
    <section id="services" class="services">
      <div class="container">
        <div class="row">
            {% for research_project in site.research_projects %}
                <div class="col-md-6 col-lg-3 d-flex align-items-stretch mb-5 mb-lg-0">
                    <div class="icon-box" data-aos="fade-up">
                    <div class="icon">{{ research_project.icon }}</div>
                            <h4 class="title"><a href="{{ research_project.url }}">{{ research_project.title }}</a></h4>
                                <p class="description">{{ research_project.description | markdownify }}</p>
                    </div>
                </div>
            {% endfor %}     
        </div>
      </div>
    </section><!-- End Research Section -->

</body>

</html>