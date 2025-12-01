---
layout: default
permalink: /repositories/
title: code
description: Open-source tools for environmental biogeochemistry research
nav: true
nav_order: 4
---

# Research Software & Tools

Our lab develops open-source software for environmental biogeochemistry research, with a focus on mass spectrometry data analysis and reactive transport modeling. All tools are freely available and contributions are welcome.

---

<section aria-labelledby="featured-projects">
  <h2 id="featured-projects">Featured Projects</h2>

  <div class="repositories featured-grid" role="list">
    {% for project in site.data.repositories.featured_projects %}
      {% include repository/repo_card.liquid project=project featured=true %}
    {% endfor %}
  </div>
</section>

<section aria-labelledby="data-analysis">
  <h2 id="data-analysis">Data Analysis Tools</h2>
  <p class="section-intro">Mass spectrometry and analytical chemistry data processing pipelines</p>

  <div class="repositories" role="list">
    {% for project in site.data.repositories.data_analysis_tools %}
      {% include repository/repo_card.liquid project=project %}
    {% endfor %}
  </div>
</section>

<section aria-labelledby="modeling">
  <h2 id="modeling">Modeling & Simulation</h2>
  <p class="section-intro">Reactive transport and biogeochemical modeling tools</p>

  <div class="repositories" role="list">
    {% for project in site.data.repositories.modeling_tools %}
      {% include repository/repo_card.liquid project=project %}
    {% endfor %}
  </div>
</section>

<section aria-labelledby="utilities">
  <h2 id="utilities">Utilities & Infrastructure</h2>
  <p class="section-intro">Supporting tools and reproducible computational environments</p>

  <div class="repositories" role="list">
    {% for project in site.data.repositories.utilities %}
      {% include repository/repo_card.liquid project=project %}
    {% endfor %}
  </div>
</section>

---

## Collaborate With Us

### Using Our Tools?
We welcome collaborations and contributions! If you're using our software:

- ⭐ **Star the repository** to show your support
- 📝 **Cite our work** in publications
- 🐛 **Report issues** or request features
- 🔧 **Contribute** code improvements via pull requests

### Contact
For collaboration inquiries or questions about our software, reach out to [cdewey@udel.edu](mailto:cdewey@udel.edu)


