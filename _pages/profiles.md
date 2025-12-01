---
layout: default
permalink: /people/
title: people
description: Meet our research team studying environmental biogeochemistry
nav: true
nav_order: 2
social: true
---

# Research Team

Our interdisciplinary team combines expertise in analytical chemistry, environmental engineering, and biogeochemistry to study how climate and land-use change affect environmental systems. We work collaboratively across field investigations, laboratory analysis, and computational modeling.

---

<section aria-labelledby="principal-investigator">
  <h2 id="principal-investigator">Principal Investigator</h2>

  <div class="team-grid" role="list">
    {% assign pi = site.data.team.principal_investigator %}
    {% capture pi_content %}{% include_relative about_cdewey.md %}{% endcapture %}
    {% assign pi_with_content = pi | merge: {'content': pi_content} %}
    {% include team/team_card.liquid member=pi_with_content %}
  </div>
</section>

<section aria-labelledby="postdocs">
  <h2 id="postdocs">Postdoctoral Researchers</h2>

  <div class="team-grid" role="list">
    {% for member in site.data.team.postdocs %}
      {% capture member_content %}{% include_relative about_mmorey.md %}{% endcapture %}
      {% assign member_with_content = member | merge: {'content': member_content} %}
      {% include team/team_card.liquid member=member_with_content %}
    {% endfor %}
  </div>
</section>

<section aria-labelledby="phd-students">
  <h2 id="phd-students">PhD Students</h2>

  <div class="team-grid" role="list">
    {% for member in site.data.team.phd_students %}
      {% if member.name == "Alex Stovall" %}
        {% capture member_content %}{% include_relative about_astovall.md %}{% endcapture %}
      {% elsif member.name == "Micah Ford" %}
        {% capture member_content %}{% include_relative about_mford.md %}{% endcapture %}
      {% endif %}
      {% assign member_with_content = member | merge: {'content': member_content} %}
      {% include team/team_card.liquid member=member_with_content %}
    {% endfor %}
  </div>
</section>

---

## Join Our Team

We welcome motivated students and postdocs interested in environmental biogeochemistry. Current opportunities include projects on wetland carbon cycling, dissolved organic matter dynamics, and reactive transport modeling. For inquiries about joining the lab, contact [cdewey@udel.edu](mailto:cdewey@udel.edu).
