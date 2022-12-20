---
layout: page
permalink: /miscellaneous/
title: miscellaneous
description: miscellaneous activities.
nav: true
importance: 6
---

<html>

          
<div class="news">
  <h2>all news</h2>
  {% if site.news != blank -%} 
  {%- assign news_size = site.news | size -%}
  <div class="table-responsive">
    <table class="table table-sm table-borderless">
    {%- assign news = site.news | reverse -%}
    {% if site.news_limit %}
    {% assign news_limit = 500 %}
    {% else %}
    {% assign news_limit = news_size %}
    {% endif %}
    {% for item in news limit: news_limit %}
      <tr>
        <th scope="row abbr"> <abbr class="badge"><span style="color:#000000">{{ item.date | date: "%b %Y" }}</span></abbr></th> 
        <td>
          {% if item.inline -%} 
            {{ item.content | remove: '<p>' | remove: '</p>' | emojify }}
          {%- else -%} 
          <a class="news-title" href="{{ item.url | relative_url }}">{{ item.title }}</a>
          {%- endif %} 
        </td>
      </tr>
      {%- endfor %} 
      </table>
  </div>
  {%- else -%} 
    <p>No news so far...</p>
  {%- endif %} 
  <h2>activities</h2>
  <div class="table-responsive">
    <table class="table table-sm table-borderless">
      <tbody>
        <tr>
          <td>volunteer</td>
          <td><a href="https://coling2020.org/">COLING 2020</a>, <a href="https://acl2020.org/">ACL 2020</a></td>
        </tr>
        <tr>
          <td>reviewer</td>
          <td><a href="https://sites.google.com/view/broadening-collaboration-in-ml/home?authuser=0">Broadening Research Collaborations in ML, NeurIPS 2022 (PC Member)</a>, <a href="https://2022.emnlp.org/">EMNLP 2022</a></td>
        </tr>
	    </tbody>
    </table>
  </div>
</div>


</html>