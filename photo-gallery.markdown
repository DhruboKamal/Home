---
layout: page
title: Gallery
permalink: /gallery/
images:
  - image_path: https://upload.wikimedia.org/wikipedia/commons/thumb/b/b6/Image_created_with_a_mobile_phone.png/1200px-Image_created_with_a_mobile_phone.png
    title: img
  - image_path: https://cdn.pixabay.com/photo/2015/04/23/22/00/tree-736885__340.jpg
    title: img2
  - image_path: /images/aus.jpg
    title: aus
---
<style>
    .photo-galary{
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
    }
    img{
        width: 450px;
        height: 300px;
        border: 1px;
        margin: 10px;
    }
</style>
<ul class= "photo-galary">
  {% for image in page.images %}
    <li>
        <img src="{{image.image_path}}" alt="{{image.title}}">
    </li>

  {% endfor %}
</ul>
