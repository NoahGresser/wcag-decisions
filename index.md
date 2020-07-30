---
  altLangPrefix: index
  contentTitle: AAACT WCAG Interpretation Decisions
  lang: en
  section: message
  title: AAACT WCAG Interpretation Decisions
  dateModified: 2020-07-29
---

## About this site

This proof-of-concept aims to clarify how WCAG 2.1 success criteria are interpreted and tested by the AAACT digital accessibility team when producing accessibility conformance reports (ACRs). It will document decisions made by the team to resolve ambiguity of WCAG success criteria, both generally and in specific scenarios.

This will be a living document, and decisions can be changed or amended at any time based on discussions in the Issues tracker or otherwise, to reflect current best practices.

You are encouraged to contribute to this document. Join the discussion, in either official language, at the link below:

[GitHub issues tracker](https://github.com/aaact-aatia/wcag-decisions/issues)

## Decisions

<nav>
{% for somepage in site.pages %}
  {% unless page.title == somepage.title or page.lang != somepage.lang %}
  <li class="item">
    <a href="{{somepage.url | remove_first:'/'}}">{{somepage.contentTitle}}</a>
    <!-- <p>{{somepage.description.en}}</p> -->
  </li>
  {% endunless %}
{% endfor %}
</nav>
