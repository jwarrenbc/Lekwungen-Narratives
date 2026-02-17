---
layout: default
header_type: base
title: Lək̓ʷáŋən Narratives
---

This is an archive of recordings of **Lək̓ʷáŋən Elder Sophie Misheal** made by Marjorie Mitchell and Barabara Efrat. They were [digitized and transcribed by Timothy Montler](https://lekwungen.montler.net/) and set in [ReadAlongStudio](https://readalong-studio.mothertongues.org/) by Jared Warren.

***

<div class="container-fluid">
  <div class="row">
    {% for project in site.data.projects %}
    <div class="col-12 col-md-6 col-lg-4 mb-4">
      <div class="card h-100 border-0 shadow-sm">
        {% if project.image %}
        <a href="{{ project.url | relative_url }}">
          <img src="{{ project.image | relative_url }}" class="card-img-top" alt="{{ project.title }}" style="object-fit: cover; height: 200px;">
        </a>
        {% endif %}
        
        <div class="card-body">
          <h5 class="card-title">
            <a href="{{ project.url | relative_url }}" class="text-dark">{{ project.title }}</a>
          </h5>
          {% if project.subtitle %}
          <p class="card-text text-muted">{{ project.subtitle }}</p>
          {% endif %}
        </div>
        
        <div class="card-footer bg-transparent border-top-0">
          <a href="{{ project.url | relative_url }}" class="btn btn-primary btn-sm btn-block">Listen & Read</a>
        </div>
      </div>
    </div>
    {% endfor %}
  </div>
</div>
