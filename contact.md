---
layout: default
title: Contact
permalink: /contact/
---

<div class="contact-grid">
  <div>
    <h2>Get in Touch</h2>
    <p><strong>{{ site.pi_name }}</strong><br>Principal Investigator</p>
    <p><a href="mailto:{{ site.email }}">{{ site.email }}</a></p>
    <h2>Address</h2>
    <p>{{ site.title }}<br>{{ site.department }}<br>{{ site.address | newline_to_br }}</p>
  </div>
  <div>
    <!-- Optional: replace with a Google Maps embed of your building -->
    <iframe
      title="Map of University of Rhode Island"
      src="https://www.google.com/maps?q=University+of+Rhode+Island,+Kingston,+RI&output=embed"
      loading="lazy"
      class="map"></iframe>
  </div>
</div>
