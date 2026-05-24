---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: splash
permalink: /
header:
    overlay_color: "#000"
    overlay_filter: "0.3"
    overlay_image: /assets/images/frontpage_pic1.jpg
    actions:
    - label: "About Me"
      url: "/about/"
excerpt: "A bioinformatician with a molecular biology background."
#author_profile: true
---
<script>
document.addEventListener("DOMContentLoaded", function() {
  const images = [
    "/assets/images/frontpage_pic1.jpg",
    "/assets/images/frontpage_pic2.jpg",
    "/assets/images/frontpage_pic3.jpg"
  ];

  let i = 0;
  const hero = document.querySelector(".page__hero--overlay");

  if (!hero) {
    console.error("Hero element not found!");
    return;
  }

  setInterval(() => {
    hero.style.opacity = "0";
    setTimeout(() => {
      i = (i + 1) % images.length;
      hero.style.backgroundImage = `url(${images[i]})`;
      hero.style.opacity = "1";
    }, 1000);
  }, 5000);
});
</script>