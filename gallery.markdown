---
layout: page
title: Gallery
permalink: /gallery/
images:
  - image_path: assets/glr001.jpg
    title: img
  - image_path: assets/glr002.jpg
    title: img
  - image_path: assets/glr003.jpg
    title: img
  - image_path: assets/glr004.jpg
    title: img
  - image_path: /assets/glr005.jpg
    title: img
  - image_path: /assets/glr006.jpg
    title: img
---

<body>
<!-- Gallery Begins -->
    <h1> Gallery </h1>
    <div class="container" style="display: flex; flex-wrap: wrap; justify-content: center">

        {% for image in page.images %}
              <img style="display: block;max-width:320px;max-height:240px;width: auto; height: auto; margin:10px;" src=" {{ image.image_path | relative_url}}" alt="...">
        {% endfor %}

    </div>
    <!--Gallery Ends -->
</body>
