---
title: Experience
layout: page
permalink: /experience/
order: 4 # Controls the order in the sidebar navigation
---

## Professional Experience

Details of my internships, full-time roles, and significant work experiences.

<div class="experience-list">
  {% assign sorted_experience = site.experience | sort: "order" %}
  {% for entry in sorted_experience %}
    <div class="experience-item mb-5 p-3 border rounded shadow-sm bg-light">
      <h3 class="fw-bold mb-1">{{ entry.title }}</h3>
      <h4 class="text-primary mb-1">{{ entry.company }}</h4>
      <p class="text-muted mb-2">{{ entry.period }} • {{ entry.location }}</p>
      <div class="experience-content">
        {{ entry.content | markdownify }} {# Renders content from the Markdown file #}

        {% if entry.responsibilities %}
          <h5 class="fw-bold mt-3">Key Responsibilities & Achievements:</h5>
          <ul class="list-unstyled small">
            {% for resp in entry.responsibilities %}
              <li><i class="fas fa-cogs me-2"></i>{{ resp }}</li>
            {% endfor %}
          </ul>
        {% endif %}

        {% if entry.links %}
          <div class="experience-links mt-3">
            {% for link in entry.links %}
              <a href="{{ link.url }}" target="_blank" rel="noopener noreferrer" class="btn btn-sm btn-outline-primary me-2 mb-2">
                <i class="fas fa-link me-1"></i> {{ link.name }}
              </a>
            {% endfor %}
          </div>
        {% endif %}
      </div>
    </div>
  {% endfor %}
</div>

<style>
  .experience-list .experience-item {
    border-left: 5px solid var(--secondary-color) !important;
    padding-left: 20px !important;
  }
  .experience-item h3 {
    font-size: 1.4rem;
  }
  .experience-item h4 {
    font-size: 1.1rem;
  }
  .experience-content ul {
    list-style: none;
    padding-left: 0;
  }
  .experience-content ul li {
    margin-bottom: 5px;
  }
  .experience-content ul li i {
    color: var(--secondary-color);
  }
</style>
