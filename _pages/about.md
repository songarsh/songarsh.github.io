---
layout: about
title: about
permalink: /
subtitle: M.Sc. student · <a href='https://safari.ethz.ch/' target='_blank'>SAFARI Research Group</a>, <a href='https://ethz.ch/' target='_blank'>ETH Zürich</a>

profile:
  align: right
  image: prof_pic.jpg
  image_circular: true
  more_info: >
    <p>CAB G 86.2</p>
    <p>Universitätstrasse 6</p>
    <p>8092 Zürich, Switzerland</p>

selected_papers: true
social: true

announcements:
  enabled: true
  scrollable: true
  limit:

latest_posts:
  enabled: false
  scrollable: true
  limit: 3
---

I am a Master's student at [ETH Zürich](https://ethz.ch/), working with the [SAFARI Research Group](https://safari.ethz.ch/) led by [Prof. Onur Mutlu](https://people.inf.ethz.ch/omutlu/).

My research focuses on **computer architecture**, with particular interest in **reconfigurable systems** and **sustainable memory systems**. I am especially excited about rethinking the memory hierarchy — DRAM, HBM, and emerging memory technologies — to make future computing systems more capable, efficient, and environmentally responsible.

Before ETH, I worked at the **Samsung Advanced Institute of Technology — India (SAIT)** on architecting dedicated compute for AI, and earned my B.E. in Electronics & Communication Engineering from **R. V. College of Engineering**, where I led the electrical module of the Formula SAE team [Ashwa Mobility Foundation](https://www.ashwarvce.com/).

Reach me at <span class="ob-mail" data-u="cy5oYXJzaDMzLmhz" data-d="Z21haWwuY29t">[email&nbsp;hidden — JS required]</span> — best for any conversation about memory systems, hardware research, or related topics.

<script>
  /* Render the address in the "user [AT] domain" format that konkanello uses,
     but keep the source HTML free of any literal email so naive crawlers
     can't harvest it. JavaScript-disabled visitors see a clear notice. */
  document.addEventListener("DOMContentLoaded", function () {
    document.querySelectorAll(".ob-mail").forEach(function (el) {
      try {
        var u = atob(el.dataset.u).split(".").join(" [DOT] ");
        var d = atob(el.dataset.d).split(".").join(" [DOT] ");
        el.textContent = u + " [AT] " + d;
      } catch (e) { /* leave placeholder */ }
    });
  });
</script>
