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

```
Could not find compatible versions

    Because every version of jekyll-default-layout depends on jekyll ~> 3.0
      and github-pages >= 107 depends on jekyll-default-layout = 0.1.4,
      github-pages >= 107 requires jekyll ~> 3.0.
    And because github-pages >= 28, < 44 depends on jekyll = 2.4.0,
      github-pages >= 28, < 44 OR >= 107 requires jekyll = 2.4.0 OR ~> 3.0.
    Because github-pages >= 44, < 147 depends on liquid = 3.0.6
      and jekyll >= 3.5.0 depends on liquid ~> 4.0,
      github-pages >= 44, < 147 is incompatible with jekyll >= 3.5.0.
    Thus, jekyll >= 4.A is incompatible with github-pages >= 28.
(1) So, because jekyll-scholar >= 6.0.0 depends on jekyll ~> 4.0,
      jekyll-scholar >= 6.0.0 is incompatible with github-pages >= 28.

    Because github-pages < 9 depends on kramdown = 1.0.2
      and github-pages >= 9, < 14 depends on kramdown = 1.2.0,
      github-pages < 14 requires kramdown = 1.0.2 OR = 1.2.0.
    And because github-pages >= 14, < 32 depends on kramdown = 1.3.1,
      github-pages < 32 requires kramdown = 1.0.2 OR = 1.2.0 OR = 1.3.1.
And because jekyll-scholar >= 6.0.0 is incompatible with github-pages >= 28
(1),
      jekyll-scholar >= 6.0.0 requires kramdown = 1.0.2 OR = 1.2.0 OR = 1.3.1.
    And because every version of kramdown-parser-gfm depends on kramdown ~> 2.0,
      jekyll-scholar >= 6.0.0 is incompatible with kramdown-parser-gfm >= 0.
    So, because Gemfile depends on kramdown-parser-gfm ~> 1.1.0
      and Gemfile depends on jekyll-scholar ~> 7.1.3,
```

{% bibliography -f {{cite_post}} --cited --prefix jekyll_github %}

