---
title: Islamic Scripture Typesetting Project
date: 2024-01-22
---

## Epub template
Fonts to embed:

```yaml
epub-fonts:
 - /usr/share/fonts/TTF/ScheherazadeNew-Bold.ttf
 - /usr/share/fonts/TTF/ScheherazadeNew-Medium.ttf
 - /usr/share/fonts/TTF/ScheherazadeNew-Regular.ttf
 - /usr/share/fonts/TTF/ScheherazadeNew-SemiBold.ttf
```

Add to Pandoc default [epub.css](https://github.com/jgm/pandoc/blob/main/data/epub.css):
```css
@font-face {
   font-family: ScheherazadeNew;
   font-style: normal;
   font-weight: normal;
   src:url("/usr/share/fonts/TTF/ScheherazadeNew-Regular.ttf");
}
@font-face {
   font-family: ScheherazadeNew;
   font-style: normal;
   font-weight: bold;
   src:url("/usr/share/fonts/TTF/ScheherazadeNew-Bold.ttf");
}
@font-face {
   font-family: ScheherazadeNew;
   font-style: italic;
   font-weight: normal;
   src:url("/usr/share/fonts/TTF/ScheherazadeNew-SemiBold.ttf");
}
@font-face {
   font-family: ScheherazadeNew;
   font-style: italic;
   font-weight: bold;
   src:url("/usr/share/fonts/TTF/ScheherazadeNew-Medium.ttf");
}

body {
	direction: rtl;
	font-family: "ScheherazadeNew";
}
```

## Resources
* https://github.com/rockneverdies55/quran-epub
