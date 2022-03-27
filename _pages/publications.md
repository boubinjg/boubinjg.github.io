---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

This page serves mainly for web-crawlers to more easily find my publications.

For humans who have stumbled upon this page, you can also find my articles on <u><a href="https://scholar.google.com/citations?user=JwIpWcwAAAAJ&hl=en">my Google Scholar profile</a></u>, or referenced in my <u><a href="/files/CV.pdf">CV</a></u>.

Here are links to some of my papers:
{% include base_path %}

{% for pdf in site.static_files %}
  {% if pdf.path contains "papers/" %}
    {% include pub.html %}
  {% endif %}
{% endfor %}


{% comment %}
#{% loop_directory directory:papers iterator:paper filter:*.pdf sort:descending %}
#    <p> paper <p>>
#{% endloop_directory %}

#{% for post in papers reversed %}
#  {% include archive-single.html %}
#{% endfor %}
{% endcomment %}
