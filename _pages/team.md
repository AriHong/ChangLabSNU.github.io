---
title: "CHANGlab - Team"
layout: gridlay
excerpt: "CHANGlab: Team members"
sitemap: false
permalink: /team/
---

## Group Members

### Principal investigator
{% assign member_list = site.data.team_pi %}
{% include team_list.html %}

### Staff
{% assign member_list = site.data.team_staff %}
{% include team_list.html %}


### Graduate students
{% assign member_list = site.data.team_graduate %}
{% include team_list.html %}


### Undergraduate students
{% assign member_list = site.data.visitors %}
{% include team_list.html %}

<script>
$('body').on('click', '.member-list-item[data-href]', function(){
    if (window.location.hash) {
        window.location.hash = $(this).data('href');
    } else {
        window.location.href = $(this).data('href');
    }
})
</script>
