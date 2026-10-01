---
title: "Home"
layout: homelay
permalink: /
---

<h1 class="home-hero">{{ site.name }}</h1>
<!-- <p class="home-hero-sub">{{ site.title }}, {{ site.institution }}</p> -->
<p class="home-hero-sub">PhD Student, Medical Imaging AI Researcher</p>


I am a PhD student at CORAL Lab, University of Maryland, Baltimore County, and I am advised by <a href="https://www.csee.umbc.edu/people/tenure-track-faculty/tim-oates/">Dr. Tim Oates</a>. I am broadly interested in all things Computer Vision, and I specialize in Medical Imaging. Currently my area of research is quality control, reconstruction, and denoising for Medical Images, and previously I have worked on highly restrictive weakly supervised segmentation. I am also interested in developing effective multi-agent systems collaborating with humans to strategize in a team environment.
Currently, I am looking for Summer 2027 internships broadly in Medical Image Analysis.

Apart from my research, I enjoy brewing up espresso-based coffees, cycling, and cats. If you would like to contact me, please send me an email!

{% capture selected %}{% bibliography --query @*[selected=true] %}{% endcapture %}
{% if selected contains "pub-entry" %}
## Selected publications

<div class="section-card selected-pubs" markdown="0">
{{ selected }}
<p style="margin: var(--space-4) 0 0;"><a href="{{ '/publications' | relative_url }}">All publications &rarr;</a></p>
</div>
{% endif %}

<!-- ## About me

Your biography goes here. The README shows how to add research-area chips, callout boxes, and a banner image. -->
