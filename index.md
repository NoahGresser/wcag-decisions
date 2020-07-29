---
  altLangPrefix: index
  contentTitle: AAACT WCAG Interpretation Decisions
  lang: en
  section: message
  title: AAACT WCAG Interpretation Decisions
  dateModified: 2020-07-29
---

## About this site

This site clarifies how WCAG 2.1 success criteria are interpreted and tested by the AAACT digital accessibility team when producing accessibility conformance reports (ACRs). It documents decisions made by the team to resolve ambiguity of WCAG success criteria, both generally and in specific scenarios.

This is a living document, and decisions can be changed or amended at any time. All changes are tracked in GitHub. ACRs are consistent with the decisions documented here at the time the ACR was produced, and will not be updated to reflect changes in these interpretations.

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