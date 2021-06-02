---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="/assets/css/style.css">
    <link rel="icon" type="image/png" href="/assets/img/favicon.ico">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
    <title>From Roots To Halo</title>
</head>

<h3>Latest Post</h3>
     <h2> <a href="{{ post.url }}">{{ post.title }}</a></h2>

  <ul>
    {% for post in site.posts limit:1 %}
     <h2> <a href="{{ post.url }}">{{ post.title }}</a></h2>
      <p>{{post.content}}</p>
    {% endfor %}
  </ul>
  <hr>
<br>
<div class="latest-list">
  <!--<h4>Recent Posts</h4>
  {% for post in site.posts limit:5 %}
          <h3> <a href="{{ post.url }}">{{ post.title }} </a></h3>
{% endfor %}-->
</div>