---
layout: default
title: Your Name - Resume
---

<div class="jumbotron">
  <h1 class="display-4">{{ page.title }}</h1>
  <p class="lead">Your tagline or personal branding statement goes here</p>
</div>

<div class="container">
  <div class="row">
    <div class="col-md-3">
      <h2>Contact Information</h2>
      <ul>
        <li>Your Name</li>
        <li>Email: your.email@example.com</li>
        <li>Phone: (123) 456-7890</li>
        <li>Location: City, State</li>
      </ul>
    </div>
    <div class="col-md-9">
      <h2>Work Experience</h2>
      <ul>
        {% for job in site.data.jobs %}
        <li>
          <h3>{{ job.title }} at {{ job.company }}</h3>
          <p><em>{{ job.start_date }} - {{ job.end_date }}</em></p>
          <p>{{ job.description }}</p>
        </li>
        {% endfor %}
      </ul>
    </div>
  </div>
</div>
