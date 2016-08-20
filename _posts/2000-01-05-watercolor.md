---
title: "Watercolors"
bg: '#666'
color: white
fa-icon: plug
image_path: http://www.ghmgallery.com/images
thumb_path: http://www.ghmgallery.com/images
images:
  - image_file: PurplePerfection.jpg
    thumb_file: PurplePerfection_thumb.jpg
    thumb_width: 120
    thumb_height: 76
    title: Purple Perfection
    year: 2016
    media_type: Watercolor and pencil
    media_width: 21
    media_height: 13
    status: Private Collection -- Prints Available
    notes:
    tags: #blue #grapes #donkey #cart #vinyard
  - image_file: PeeringIntoFall.jpg 
    thumb_file: PeeringIntoFall_thumb.jpg
    thumb_width: 60
    thumb_height: 80
    title: Peering into Fall
    year: 2015
    media_type: Watercolor
    media_width: 30
    media_height: 22
    status: 
    notes:
    tags: #orange #leaves #azelia #fallseason
---
<a name="watercolors"></a>
<!-- {% if image.thumb_height %}height="80"{% endif %}" -->
<ul class="photo-gallery">
  {% for image in page.images %}
    <a target="_blank" href="{{ page.image_path }}/{{ image.image_file }}">
    <img align="right" src="{{ page.thumb_path }}/{{ image.thumb_file }}"
      {% if image.thumb_width %}width="{{ image.thumb_width }}"{% endif %}
      {% if image.thumb_height %}height="{{ image.thumb_height }}"{% endif %}
    alt='{{ image.media_type }}: {{ image.title }} {{ image.tags }}'> 
    <strong><em>{{ image.title }}</em></strong>. {{ image.year }}. 
    {{ image.media_type }}. {{ image.media_width }}x{{ image.media_height }} inches.
    <br />{{ image.status }} {{ image.notes }}
    </a><br style="clear: both;" /><br />
  {% endfor %}
</ul>

TODO: Show tags in smaller font
