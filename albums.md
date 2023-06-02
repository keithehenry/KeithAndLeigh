---
title: Photos & Videos
layout: page
permalink: /albums/
sub_title: "Some of our favorite photo albums and video slideshows. Enjoy!"
introduction: |
    *Click the image to see the album at Google Photos or video at YouTube.*
---

<div class="entries-grid">
  {% assign ordered_albums = site.albums | sort:"title" %}
  {% for album in ordered_albums reversed %}
    <div class="album">
      <h3>{{ album.title }}</h3>
      {{ album.content }}
    </div>
  {% endfor %}
</div>
