---
layout: page
title: "Quantum Machine Learning Research Group"
permalink: /team/
---

# Quantum Machine Learning Lab Team
## Our Mission
Briefly describe the mission or main research focus of the lab.

## Principal Investigator
![PI's Image](./../images/oross-pic.jpg)  
**Name**: PhD Oscar Humberto Montiel Ross  
**Position**: Principal Investigator  
**Research Interests**: Quantum Computing, Artificial Intelligence
**Contact**: oross@citedi.mx

## Team Members

{% include base_path %}
{% for member in site.data.lab_team %}
<div class="team-member">
    <div class="member__avatar">
        {% if member.avatar contains "://" %}
            <img src="{{ member.avatar }}" alt="{{ member.name }}">
        {% else %}
            <img src="{{ member.avatar | prepend: '/images/' | prepend: base_path }}" alt="{{ member.name }}">
        {% endif %}
    </div>
    <div class="member__content">
        <h3 class="member__name">{{ member.name }}</h3>
        <p class="member__position">{{ member.position }}</p>
        <p class="member__research_interests">{{ member.research_interests }}</p>
        <p class="member__contact">{{ member.contact }}</p>
    </div>
</div>
{% endfor %}

## Research Areas
Describe the main research areas of the lab, possibly with sub-sections for each area.

## Publications
List recent publications with links to them, if available.

## Join Us
Information on open positions, how to apply, and what qualities you're looking for in candidates.

## Contact Us
Lab address, email, and any other contact information.
