---
title: "Jekyll과 Jekyll Theme으로 Github Page 만들기"
tags:
  - Github Pages
  - Jekyll
  - Minimal-Mistakes
math: true
---
{% assign cite_post = 'reference.bib' %}
https://github.com/inukshuk/jekyll-scholar/issues/203
## Github Pages
a{% cite ruby -f {{cite_post}} --prefix jekyll_github%}
```html
1. [1]D. Flanagan and Y. Matsumoto, The Ruby Programming Language. O’Reilly Media, 2008.
```

```html
<!-- Bibliography -->
  <bibliography entry-spacing="0" second-field-align="flush">
    <layout>
      <!-- Citation Number -->
      <text variable="citation-number" prefix="[" suffix="] "/>
```

```html
1. [1] D. Flanagan and Y. Matsumoto, The Ruby Programming Language. O’Reilly Media, 2008.
```

```
 • [1] D. Flanagan and Y. Matsumoto, The Ruby Programming Language. O’Reilly Media, 2008.
```
{% bibliography -f {{cite_post}} --cited --prefix jekyll_github %}

