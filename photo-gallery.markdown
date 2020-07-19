---
layout: page
title: Image Gallery
permalink: /gallery/
images:
  - image_path: /cca1.jpg
    title: australs
---
<ul class= "photo-galary">
  {% for image in page.images %}
    <li>
        <img src="{{imgage.image_path}}" alt="{{image.title}}">
    </li>

  {% endfor %}
</ul>
