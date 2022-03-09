# Hi! I’m Deanna,
### a graduate student at Simmons University.

I aim to graduate with two degrees, a **Master of Science in Archives** and a **Master of Arts in History**, by May 2023. In addition to archival studies, I have professional experience with *data analysis*, *database management*, *front-end web development*, *mailing lists*, and *copy editing*.

This site hosts examples of academic achievements, a current (work in progress) resume, and contact information for professional inquiries.

## Portfolio
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>
