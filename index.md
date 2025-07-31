---
layout: home
title: "دفتر الحكايات"
excerpt: "مرحباً بكم في مدونة دفتر الحكايات حيث تجدون قصصاً ومقالات تعليمية مبسطة."
author_profile: true
header:
  overlay_color: "#000"
  overlay_filter: "0.3"
  overlay_image: "/assets/images/header-bg.jpg"  # (يمكنك وضع صورة خلفية هنا)
  cta_label: "ابدأ القراءة"
  cta_url: "/year-archive/"
  caption: "قصص ومقالات تعليمية"
---

## ✨ جديد المدونة
مرحباً بك في عالم الحكايات والمعرفة! في هذه المدونة، ستجد مقالات وقصصاً تعليمية مكتوبة بأسلوب مبسط وشيق لتساعدك في تنمية مهاراتك وفهمك للأشياء حولك.

---

{% if paginator.posts %}
  {% for post in paginator.posts %}
  ### [{{ post.title }}]({{ post.url | relative_url }})
  {{ post.excerpt | markdownify }}
  ---
  {% endfor %}
{% endif %}
