---
layout: page
title: About
permalink: /about/
---

<!-- TODO: write your About page here. Plain Markdown works. -->

My name is William Fincher. I am a <span id="age" data-born="2000-08-31">26</span> year old Law student and nonprofit-employee, who has four years of experience in nonprofit adminstrative functions, such as, HR, Operations, Facilities, and programmatic support at a non-profit school. I am deeply concerned about the way we move throughout this world and what the future holds, and I hope to reflect on that to some degree on this website. 

<script>
  // Keep the age current: count full years since the birth date.
  (function () {
    var el = document.getElementById('age');
    var born = new Date(el.dataset.born + 'T00:00:00');
    var now = new Date();
    var age = now.getFullYear() - born.getFullYear();
    if (now.getMonth() < born.getMonth() ||
        (now.getMonth() === born.getMonth() && now.getDate() < born.getDate())) age--;
    el.textContent = age;
  })();
</script>
