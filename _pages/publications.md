---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}
{% assign profile_pubs = site.publications | where: "profile_owner", true | sort: "date" | reverse %}

{% if profile_pubs.size > 0 %}
{% for post in profile_pubs %}
### [{{ post.title }}]({{ post.url | prepend: base_path }})

**Authors:** {{ post.authors | default: "YiQin Hao" }}  
**Venue/Status:** {{ post.venue }}{% if post.status %}; {{ post.status }}{% endif %}  
{% if post.paperurl %}**Link:** [Paper]({{ post.paperurl }}){% endif %}

{{ post.excerpt }}

{% endfor %}
{% else %}
No publications added yet.
{% endif %}
