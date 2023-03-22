# Responsive Image

Example of a responsive image partial. The image is hosted on Cloudinary. The Cloudinary URL is located in the site data, the src field below references just the image. The complete image src URL is built in the image component.

## Fields
```
mediaType: Image
...
image:
  src: "v1664225762/my-starter/Mmollis-malesuada-inceptos_xqymoo.jpg"
  alt: "Justo Elit Euismod"
  aspectRatio: "66.67"
  caption: "Duis mollis, est non commodo luctus, nisi erat porttitor."
```

## Template
```
{% macro responsiveImage(image, siteMeta) %}
  <div class="responsive-wrapper js-progressive-image-wrapper" style="padding-bottom:{{ image.aspectRatio}}%;" >

    {# assemble the image url #}
    {% set source = siteMeta.imagePrefix ~ image.src %}

    {# get image source for LRIP #}
    {% set lowResImagesrc = siteMeta.imagePrefix ~ "w_100,c_fill,g_auto,f_auto/" ~ image.src %}

    <img class="low-res" src="{{ lowResImagesrc }}" alt="{{ image.alt }}"/>
    <img class="high-res" src="" alt="{{ image.alt }}" data-prefix="{{ siteMeta.imagePrefix }}" data-source="{{ image.src }}"/>
  </div>
  <p class="caption">{{ image.caption }}</p>
{% endmacro %}
```
