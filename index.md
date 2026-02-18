---
layout: default
header_type: base
title: Lək̓ʷáŋən Narratives
copyright: "Site &copy; 2026 Jared Warren"
---

This is an archive of recordings of **Lək̓ʷáŋən Elder Sophie Misheal** made by Marjorie Mitchell and Barabara Efrat in the 1960s (note that some of the recordings contain echos of other stories). They were [digitized and transcribed by Timothy Montler](https://lekwungen.montler.net/) and set in [ReadAlongStudio](https://readalong-studio.mothertongues.org/) by Jared Warren.

***

<div class="container-fluid">
  <div class="row">
    {% for project in site.data.projects %}
    {% assign project_url = "/" | append: project.slug | append: "/www/" %}
    {% assign project_image = "/" | append: project.slug | append: "/www/assets/image-" | append: project.asset | append: "-0.jpg" %}
    <div class="col-12 col-md-6 col-lg-4 mb-4">
      <div class="card h-100 border-0 shadow-sm">
        <a href="{{ project_url | relative_url }}">
          <img src="{{ project_image | relative_url }}" class="card-img-top" alt="{{ project.title }}" style="object-fit: cover; height: 200px;">
        </a>
        
        <div class="card-body">
          <h5 class="card-title">
            <a href="{{ project_url | relative_url }}" class="text-dark">{{ project.title }}</a>
          </h5>
        </div>
        
        <div class="card-footer bg-transparent border-top-0">
          <a href="{{ project_url | relative_url }}" class="btn btn-primary btn-sm btn-block">Listen & Read</a>
        </div>
      </div>
    </div>
    {% endfor %}
  </div>
</div>
