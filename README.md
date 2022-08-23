# myLightning.network

```
minimum hugo version 0.101.0+extended
```

# Setup dev env

Configure "config.toml"

# Run hugo server

```
hugo serve -D
```

# Build hugo site

```
hugo --ignoreCache --minify
```

# To create new page

```
hugo new content/page_name.md
```

and then edit file located at "./content/page_name.md", setup frontmatter

# To create new blog post

```
hugo new content/posts/post_title.md
```

and then edit file located at "./content/posts/post_title.md", then setup
frontmatter

# Front matter breakdown

```
---
title: "Post Title" (1)
date: 2022-08-18T19:23:39+07:00 (2)
draft: false (3)
seo_description: "lorem ipsum dolor sit amet" (4)
seo_keyword: (5)
  - keyword1
  - keyword2
thumbnail: "posts/example.jpg" (6)
youtube_url: "https://www.youtube.com/watch?v=D0UnqGm_miA" (7)
audio_url: "/assets/audios/file.mp3" (8)
tags: (9)
  - tags1
  - tags2
category: (10)
  - Magazine
  - Podcast
slug: "{{ lower .Name | urlize }}" (11)
---
```

1. Set page or post title
2. Set date page or post published
3. Set draft, set to true then page or post will be hidden in production
4. Set SEO META description
5. Set SEO META keyword
6. Set thumbnail, value must be set, place image in "./static/assets/images/"
7. Set youtube URL
8. Set audio URL (for Podcast category, other than Podcast set to "")
9. Set post tags, must be set at least 1 tag
10. Set post category, must be set at least 1 category
11. Set URL slug
