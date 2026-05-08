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

I am a Master's student <span class="nowrap">at [ETH Zürich](https://ethz.ch/)</span> in the <span class="nowrap">Electrical Engineering and Information Technology</span> program, working <span class="nowrap">with the [SAFARI Research Group](https://safari.ethz.ch/)</span> <span class="nowrap">under [Prof. Onur Mutlu](https://people.inf.ethz.ch/omutlu/)</span>.

My research sits at the intersection of <span class="nowrap">**computer architecture**</span> and <span class="nowrap">**memory systems**</span>. I am particularly drawn to rethinking the memory hierarchy to make future computing both more capable and more sustainable.

Before ETH, I spent two and a half years <span class="nowrap">at **Samsung Semiconductor**</span> architecting <span class="nowrap">dedicated compute</span> <span class="nowrap">for AI</span> workloads and contributing to the <span class="nowrap">HBM-PIM near-memory architecture</span>. I earned my Bachelor's <span class="nowrap">in Electronics & Communication Engineering</span> <span class="nowrap">from **R. V. College of Engineering**, Bengaluru</span>.

Feel free to reach out — I'm always happy to chat about <span class="nowrap">memory systems</span>, <span class="nowrap">hardware research</span>, or anything in between.

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
