---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

**Note**: * indicates co-first authorships

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

## Preprints and submissions

{% for post in site.publications reversed %}
  {% if post.permalink contains "/preprints/" %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

## Journal and conference papers

{% for post in site.publications reversed %}
  {% unless post.permalink contains "/preprints/" %}
    {% include archive-single.html %}
  {% endunless %}
{% endfor %}

