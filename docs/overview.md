# Starter Documentation

This is the starter documentation for your project. It is written in Markdown. Further information may be found at https://metalsmith-components.netlify.app/.

Pages are composed with sections. Sections are defined in the frontmatter of each page.

Sections maybe composed from partials, which are defined in the `partials` folder. This is shown at the sections object outline below with a media section composed from text, ctas, video, image, lottieData, icon or audio partials.

```
---
layout: sections.njk

seo:
  title: My Metalsmith Starter
  description: "My personal starter to build a website with Metalsmith"
  socialImage: "/assets/images/metalsmith-starter-social.png"
  canonicalOverwrite: ""

sections:
  - component: banner
    ...
  - component: intro
    ...
  - component: media
    ...
    text:
      ...
    hasCtas: false
    ctas:
      ...
    mediaType: Image
    video:
      ...
    image:
      ...
    lottieData:
      ...
    icon: ""
    audio:
      ...
  - component: media
    ...
  - component: intro
    ...
---
```

All page sections are documented in a file with the name of the section, e.g. banner.md for the banner section.

