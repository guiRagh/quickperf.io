---
title: Latest Posts
permalink: /blog/
---

<ul>
  {% for post in site.posts %}
    <li>
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>

<a class="twitter-timeline" 
id="timeline"
data-tweet-limit="4"
data-chrome="transparent"
href="https://twitter.com/QuickPerf?ref_src=twsrc%5Etfw">Tweets by QuickPerf</a> 

<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

<script>
    if (theme === "dark") {
      document.getElementById("timeline").setAttribute("data-theme", "dark");
      document.getElementById("timeline").setAttribute("data-border-color", "#FFF");
    } else {
      document.getElementById("timeline").setAttribute("data-theme", "light");
      document.getElementById("timeline").setAttribute("data-border-color", "#DCDCDC");
    }
</script>