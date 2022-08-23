---
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
draft: false
seo_description: ""
seo_keyword:
  - keyword1
  - keyword2
thumbnail: "posts/example.jpg"
youtube_url: "https://www.youtube.com/watch?v=D0UnqGm_miA"
audio_url: "/assets/audios/file.mp3"
tags:
  - tags1
  - tags2
category:
  - Podcast
  - Game Theory
  - News
slug: "{{ lower .Name | urlize }}"
---

