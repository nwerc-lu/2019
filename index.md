---
layout: page
---

Follow [Lund University](https://www.lu.se/) at [NWERC 2019](https://nwerc.eu/), the north western european qualification for the World Championships in competitive programming in teams - ICPC. The contest starts at 10:00 the 17th of November and lasts for 5 hours. 

The scoreboard will be available at [https://scoreboard.nwerc.eu/](https://scoreboard.nwerc.eu/) when the contest has started, and the problems are published 30 minutes into the competition at the [open competition](https://open.kattis.com/contests/nwerc19open).

## Blog

<ul class="post-list">
{% for post in site.posts %}
 <li>
  <div id="flex-container">
   <a class="post-title" href="{{ post.url | prepend: site.baseurl }}">
    <div id="thumbnail-img">
     {% if post.img %}
     <img src="{{post.img}}"
     {% if post.portrait %} class="portrait" {% endif %}
     />
     {% else %}
     <div class="thumbnail blankbox"></div>
     {% endif %}
    
    </div>
   </a>
   <div  style="display:block;text-align:left">
    <a class="post-title" href="{{ post.url | prepend: site.baseurl }}">
     <h4>{{ post.title }}</h4>
   </a>
     <p class="post-meta">{{ post.date | date: '%B %-d, %Y' }}</p>
     <p>{{ post.description }}</p>
    </div>
  </div>
  <br/>
  <hr/>
 </li>
    
{% endfor %}
</ul>
