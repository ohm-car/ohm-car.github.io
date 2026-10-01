---
title: "Home"
layout: homelay
permalink: /
---

<h1 class="home-hero">{{ site.name }}</h1>
<!-- <p class="home-hero-sub">{{ site.title }}, {{ site.institution }}</p> -->
<!-- <p class="home-hero-sub">PhD Student, Medical Imaging AI Researcher</p> -->
<p class="home-hero-sub">I'm a researcher who designs Generative AI algorithms for denoising and recosntructing Medical Imaging</p>


I am a PhD student at CORAL Lab, University of Maryland, Baltimore County, and I am advised by <a href="https://www.csee.umbc.edu/people/tenure-track-faculty/tim-oates/">Dr. Tim Oates</a>. I am broadly interested in all things Computer Vision, and I specialize in Medical Imaging. Currently my areas of research are quality control, reconstruction, and denoising for Medical Images. The aim of my work is to reduce the need for invasive scanning for patients, and to help oncologists work with non-invasive scans (which tend to be noisy); and also to mitigate the domain shift problem, caused when medical image data from different sites (hospitals, clinics, orthopedics, etc.) is used with models that haven't seen data from these sites. In the past, I've worked on highly restrictive weakly supervised segmentation. Another area of research I am interested in is developing effective multi-agent systems collaborating with humans to strategize in a team environment.
Currently, I am looking for Summer 2027 internships broadly in Medical Image Analysis.
<!-- Prior to this, I did a Bachelor's of Engineering in Computer Science from <a href="https://www.bits-pilani.ac.in/goa">BITS Pilani</a>, and I worked as a Software Developer at Innova Systems in Hyderabad, India. -->

Apart from my research, I enjoy brewing up espresso-based coffeeswith my fancy espresso machine, long/short distance cycling, and cats (HUGE fan of cats). If you'd like to get in touch or meet, please send me an email!

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
