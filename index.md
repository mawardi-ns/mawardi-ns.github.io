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
    - label: "About Me"
    url: "/about/"
excerpt: "A bioinformatician with a molecular biology background."
#author_profile: true
---
<style>
.page__hero--overlay {
  transition: background-image 1s ease-in-out;
}
</style>

<script>
const images = [
  "/assets/images/frontpage_pic1.jpg",
  "/assets/images/frontpage_pic2.jpg",
  "/assets/images/frontpage_pic3.jpg"
];

let i = 0;
setInterval(() => {
  i = (i + 1) % images.length;
  document.querySelector(".page__hero--overlay").style.backgroundImage = `url(${images[i]})`;
}, 5000);
</script>