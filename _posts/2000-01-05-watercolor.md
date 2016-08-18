---
title: "Watercolors"
bg: '#666'
color: white
fa-icon: plug
image_path: http://www.ghmgallery.com/images
thumb_path: http://www.ghmgallery.com/images
images:
  - image_file: PeeringIntoFall.jpg	
    thumb_file: PeeringIntoFall_thumb.jpg
    title: Peering into Fall
    year: 2015
    media: Watercolor
    width: 30
    height: 22
    status: 
    notes:
  - image_file: PurplePerfection.jpg
    thumb_file: PurplePerfection_thumb.jpg
    title: Purple Perfection
    year: 2016
    media: Watercolor and pencil
    width: 21
    height: 13
    status: Private Collection -- Prints Available
    notes:
---
<a name="watercolors"></a>

<ul class="photo-gallery">
  {% for image in page.images %}
    <a target="_blank" href="{{ page.image_path }}/{{ image.image_file }}">
    <img src="{{ page.thumb_path }}/{{ image.thumb_file }}" alt="{{ image.title }}" {{ image.year }}, {{ image.width }}x{{ image.height }} {{ image.status }}  {{ image.notes }}"> "{{ image.title }}" {{ image.year }}, {{ image.width }}x{{ image.height }} {{ image.status }}  {{ image.notes }}</a><br /><br />
  {% endfor %}
</ul>
