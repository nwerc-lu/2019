---
layout: page
---

Follow [Lund University](https://www.lu.se/) at [NWERC 2019](https://nwerc.eu/), the north western european qualification for the World Championships in competitive programming in teams - ICPC. The contest starts at 10:00 the 17th of November and lasts for 5 hours. 

### Training Schedule

| Date      | Link        | Competition |
|-----------|-------------|-------------|
|2019-11-03 |[Scoreboard](https://open.kattis.com/contests/jdscvz) | TBA |
|2019-11-01 |[Scoreboard](https://google19.kattis.com/) | Coding Cup @ Google 2019 |
|2019-10-27 |[Scoreboard](https://open.kattis.com/contests/imed8b) | TBA |
|2019-10-23 |[Scoreboard](https://open.kattis.com/contests/xtfb8h) | Hong Kong Regional Contest 2016 |
|2019-10-22 |[Scoreboard](https://open.kattis.com/contests/p3n9ss) | Vietnam National Programming Contest 2017 |
|2019-10-19 |[Scoreboard](https://2019.bapc.eu/results.html#bapc-semi-live-contest-results) | Benelux Algorithm Programming Contest 2019 |
|2019-10-16 |[Scoreboard](https://open.kattis.com/contests/wybxdy) | IDI Open 2019 |

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
