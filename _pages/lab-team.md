---
layout: page
title: "Quantum Machine Learning Research Group"
permalink: /team/
---

<header class="banner">
  <img src="./../images/quantum-computer-banner.jpg" alt="Quantum Machine Learning">
</header>

<div class="team-header">
  <h1>Team</h1>
</div>

{% include base_path %}
{% for member in site.data.lab-team %}
<div class="team-member">
    <h1 class="member__position">{{ member.position }}</h1>
    <div class="member__avatar">
        <a href="{{ site.baseurl }}/team/{{ member.profile_slug }}" >
            {% if member.avatar contains "://" %}
                <img src="{{ member.avatar }}" alt="{{ member.name }}">
            {% elsif member.avatar %}
                <img src="{{ member.avatar | prepend: '/images/' | prepend: base_path }}" alt="{{ member.name }}">
            {% else %}
                <img src="{{ '/images/blank-profile.png' | prepend: base_path }}" alt="Default Avatar">
            {% endif %}
        </a>
    </div>
    <div class="member__info">
        <h3 class="member__name">{{ member.name }}</h3>
    </div>
    <div class="member__content">
        <p class="member__abstract">{{ member.abstract }}</p>
    </div>
</div>
{% endfor %}

## Join Us
Information on open positions, how to apply, and what qualities you're looking for in candidates.

## Contact Us
Lab address, email, and any other contact information.
