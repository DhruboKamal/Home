---
layout: page
title: Image Gallery
permalink: /gallery/
images:
  - image_path: https://upload.wikimedia.org/wikipedia/commons/thumb/b/b6/Image_created_with_a_mobile_phone.png/1200px-Image_created_with_a_mobile_phone.png
    title: img
  - image_path: /images/aus.jpg
    title: aus
---
<ul class= "photo-galary">
  {% for image in page.images %}
    <li>
        <img src="{{image.image_path}}" alt="{{image.title}}">
    </li>

  {% endfor %}
</ul>
