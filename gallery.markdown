---
layout: gallery
title: Gallery
permalink: /gallery/
images:
  - image_path: https://upload.wikimedia.org/wikipedia/commons/thumb/b/b6/Image_created_with_a_mobile_phone.png/1200px-Image_created_with_a_mobile_phone.png
    title: img
  - image_path: https://cdn.pixabay.com/photo/2015/04/23/22/00/tree-736885__340.jpg
    title: img2
  - image_path: https://upload.wikimedia.org/wikipedia/commons/thumb/b/b6/Image_created_with_a_mobile_phone.png/1200px-Image_created_with_a_mobile_phone.png
    title: img3
  - image_path: https://cdn.pixabay.com/photo/2015/04/23/22/00/tree-736885__340.jpg
    title: img4

---

<body>
<!-- Gallery Begins -->
    <h1> Gallery </h1>
    <div class="container" style="display: flex; flex-wrap: wrap; justify-content: center">

        {% for image in page.images %}
              <img style="height: 240px;width: 320px;margin:10px;" src=" {{image.image_path | relative_url}}" alt="...">
        {% endfor %}

    </div>
    <!--Gallery Ends -->
</body>
