---
layout: default
lang: en
title: "Gabriel — CV & Portfolio"
description: "Personal website — choose your language"
---

<div class="card" style="text-align: center;">
    <h2>🌐 Choose your language / Choisissez votre langue / בחר שפה</h2>
    <p style="color: var(--muted); margin-bottom: 1.5rem;">
        Select your preferred language to view Gabriel's CV and portfolio.
    </p>

    <div class="lang-selector">
        {% for lang in site.data.languages %}
            {% assign l = lang[1] %}
            <a href="{{ site.baseurl }}/{{ l.code }}/" class="lang-card">
                <span class="flag">{{ l.flag }}</span>
                <span class="name">{{ l.name }}</span>
            </a>
        {% endfor %}
    </div>
</div>
