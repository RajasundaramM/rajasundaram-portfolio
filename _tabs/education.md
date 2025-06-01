---
title: Education
layout: page
permalink: /education/
order: 2 # Controls the order in the sidebar navigation
---

<div class="education-timeline">
  {% assign sorted_education = site.education | sort: "order" %}
  {% for entry in sorted_education %}
    <div class="timeline-item mb-5 p-3 border rounded shadow-sm bg-light">
      <h3 class="fw-bold mb-1">{{ entry.degree }}</h3>
      <h4 class="text-primary mb-1">{{ entry.institution }}</h4>
      <p class="text-muted mb-2">{{ entry.period }} • {{ entry.location }}</p>
      <div class="timeline-content">
        {{ entry.content | markdownify }} {# Renders content from the Markdown file #}

        {% if entry.coursework %}
          <h5 class="fw-bold mt-3">Key Coursework:</h5>
          <ul class="list-unstyled small">
            {% for course in entry.coursework %}
              <li><i class="fas fa-book me-2"></i>{{ course }}</li>
            {% endfor %}
          </ul>
        {% endif %}

        {% if entry.activities %}
          <h5 class="fw-bold mt-3">Activities & Honors:</h5>
          <ul class="list-unstyled small">
            {% for activity in entry.activities %}
              <li><i class="fas fa-award me-2"></i>{{ activity }}</li>
            {% endfor %}
          </ul>
        {% endif %}
      </div>
    </div>
  {% endfor %}
</div>

<style>
  .education-timeline .timeline-item {
    border-left: 5px solid var(--primary-color) !important;
    padding-left: 20px !important;
  }
  .timeline-item h3 {
    font-size: 1.4rem;
  }
  .timeline-item h4 {
    font-size: 1.1rem;
  }
  .timeline-content ul {
    list-style: none;
    padding-left: 0;
  }
  .timeline-content ul li {
    margin-bottom: 5px;
  }
  .timeline-content ul li i {
    color: var(--primary-color);
  }
</style>
