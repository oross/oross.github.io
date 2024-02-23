---
layout: page
title: "Quantum Machine Learning Research Group"
permalink: /team/
---

# Quantum Machine Learning Lab Team

## Team Members

{% include base_path %}
{% for member in site.data.lab-team %}
<div class="team-member">
    <h1 class="member__position">{{ member.position }}</h1>
    <div class="member__avatar">
        {% if member.avatar contains "://" %}
            <img src="{{ member.avatar }}" alt="{{ member.name }}">
        {% elsif member.avatar %}
            <img src="{{ member.avatar | prepend: '/images/' | prepend: base_path }}" alt="{{ member.name }}">
        {% else %}
            <img src="{{ '/images/blank-profile.png' | prepend: base_path }}" alt="Default Avatar">
        {% endif %}
    </div>
    <div class="member__content">
        <h3 class="member__name">{{ member.name }}</h3>
        <p class="member__abstract">{{ member.abstract }}</p>
        <a href="{{ site.baseurl }}/team/{{ member.profile_slug }}" class="profile-icon-link">
        <i class="fas fa-user-circle fa-3x"></i>
    </a>
    </div>
</div>
{% endfor %}

## Join Us
Information on open positions, how to apply, and what qualities you're looking for in candidates.

## Contact Us
Lab address, email, and any other contact information.
