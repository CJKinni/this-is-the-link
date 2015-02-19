---
layout: page
title: This is the Link
tagline: The News, Summarized
---
{% include JB/setup %}

<div class="summary">  

  {% assign post = site.posts.first %}
  {% assign content = post.content %}

  <div class="row post-full">
    <div class="col-md-12">
      <hr />
        <div class="post-header">
          <h2>For {{ post.date | date: "%A, %B %e, %Y" }}{% if post.title %}<br><small>{{post.title}}</small>{% endif %}</h2>
        </div>
        {{ content }}
    </div>
  </div>
  
</div>

