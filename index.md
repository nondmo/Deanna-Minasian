# Hi! I’m Deanna,
### a graduate student at Simmons University.

I aim to graduate with two degrees, a **Master of Science in Archives** and a **Master of Arts in History**, by May 2023. In addition to archival studies, I have professional experience with *data analysis*, *database management*, *front-end web development*, *mailing lists*, and *copy editing*.

This site hosts examples of academic achievements, a current (work in progress) resume, and contact information for professional inquiries.


## Portfolio
{% assign projects = site.data.projects | get_projects_from_files | sort:'date' %}
{% for project in projects reversed %}
    <!-- portfolio-item -->
    <h2>{{ project.title }} <span>{{ project.category | slugify }}</h2>

    <a href="/{{ project.dir }}">
        <img src="{{ project.image.url }}" alt="{{ project.image.alt }}" title="{{ project.image.title }}">
    </a>
    <!-- portfolio-item -->
{% endfor %}
