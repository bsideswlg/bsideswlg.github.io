---
layout: default
title: Home
permalink: /
---

<div class="posts">
  {% for post in paginator.posts %}
  <div class="post">
    <h1 class="post-title">
      <a href="{{ site.baseurl }}{{ post.url | remove_first: '/'}}">
        {{ post.title }}
      </a>
    </h1>

    <span class="post-date">{{ post.date | date_to_string }}</span>

    {{ post.content }}
  </div>
  {% endfor %}
</div>


# BSides Wellington

## November 23rd & 24th, 2017 at Shed 6

[Our CFP is now open until August 26, 2017!](https://www.papercall.io/bsideswlg2017)

Why not [join our public slack](https://chat.bsides.nz) or [email us](mailto:info@bsides.nz) with any inquiries you may have?

Interested in sponsoring our event? [Click and download our kit here for more info!](http://bsideswlg.github.io/sponsor/BSidesWLG_2017_Sponsorship_Kit.pdf)

You can also [follow us on twitter](https://twitter.com/bsideswlg) if you'd like to "bee" in the loop!

BSides Wellington takes pride in following our Code of Conduct. [You can read it in full here!](code-of-conduct) 

{% comment %}
<div class="pagination">
  {% if paginator.next_page %}
    <a class="pagination-item older" href="{{ site.baseurl }}page{{paginator.next_page}}">Older</a>
  {% else %}
    <span class="pagination-item older">Older</span>
  {% endif %}
  {% if paginator.previous_page %}
    {% if paginator.page == 2 %}
      <a class="pagination-item newer" href="{{ site.baseurl }}">Newer</a>
    {% else %}
      <a class="pagination-item newer" href="{{ site.baseurl }}page{{paginator.previous_page}}">Newer</a>
    {% endif %}
  {% else %}
    <span class="pagination-item newer">Newer</span>
  {% endif %}

</div>
{% endcomment %}