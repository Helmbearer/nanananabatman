---
layout: splash
title: "Team Members"
permalink: /staff-members/
entries_layout: grid
---

<div class="grid__item">
  {% for staff_member in site.staff_members %}
  <div class="staff_member">
    {% include archive-single.html type="grid" %}
    <div class="image">
    <img src = "{{site.baseurl}}/assets/members/{{staff_member.image}}" alt ="" width = "238px" height = "320px" style="float: left ;margin-right: 10px; margin-bottom: 10px;">
    </div>
    <h2>{{ staff_member.name}}</h2>
    {{staff_member.email}} <br/>
    {{staff_member.position}}<br/>
    {{staff_member.topics}} <br/>
    {{staff_member.homepage}} <br/>
    </div>
  {% endfor %} 
</div>

