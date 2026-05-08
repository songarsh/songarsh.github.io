---
layout: about
title: about
permalink: /
subtitle: <span class="nowrap">MSc Student</span> · <a href='https://safari.ethz.ch/' target='_blank' class="nowrap">SAFARI Research Group</a>, <a href='https://ethz.ch/' target='_blank' class="nowrap">ETH Zürich</a>

profile:
  align: left
  image: prof_pic.jpg
  image_circular: false
  more_info: >
    <p class="header-email"><span class="ob-mail" data-u="cy5oYXJzaDMzLmhz" data-d="Z21haWwuY29t">[email hidden — JS required]</span></p>
    <p class="header-address"><strong class="nowrap">ETZ F78</strong> · <span class="nowrap">Gloriastrasse 35</span>, <span class="nowrap">8092 Zürich</span>, Switzerland</p>
    <p class="header-address"><strong class="nowrap">OAT F16</strong> · <span class="nowrap">Andreasstrasse 5</span>, <span class="nowrap">8050 Zürich</span>, Switzerland</p>

selected_papers: true
social: true

announcements:
  enabled: true
  scrollable: true
  limit:

timeline:
  enabled: true
  scrollable: true
  reverse: true # true = newest period at the top

latest_posts:
  enabled: false
  scrollable: true
  limit: 3
---

I am a Master's student <span class="nowrap">at [ETH Zürich](https://ethz.ch/)</span>, working <span class="nowrap">with the [SAFARI Research Group](https://safari.ethz.ch/)</span> <span class="nowrap">led by [Prof. Onur Mutlu](https://people.inf.ethz.ch/omutlu/)</span>.

My research focuses <span class="nowrap">on **computer architecture**</span>, with particular interest <span class="nowrap">in **reconfigurable systems**</span> <span class="nowrap">and **sustainable memory systems**</span>. I am especially excited about rethinking the memory hierarchy — DRAM, HBM, and emerging memory technologies — to make future computing systems more capable, efficient, and environmentally responsible.

Before ETH, I worked <span class="nowrap">at **Samsung**</span> on architecting <span class="nowrap">dedicated compute</span> <span class="nowrap">for AI</span>, and earned my B.E. <span class="nowrap">in Electronics & Communication Engineering</span> <span class="nowrap">from **R. V. College of Engineering**</span>.

Feel free to reach out — happy to chat about memory systems, hardware research, or anything in between.

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
