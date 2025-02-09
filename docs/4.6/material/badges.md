---
layout: docs
title: Badges
description: Badges can contain dynamic information, such as a number of pending requests.
group: material
redirect_from:
  - /docs/4.4/material/badges/
  - /docs/4.5/material/badges/
---

<div class="list-group my-2 my-lg-5">
    <a href="{{ site.baseurl }}/docs/{{ site.docs_version }}/components/badge/" target="_blank" class="list-group-item list-group-item-action d-flex list-group-item-two-line font-weight-bold">
    <span class="list-group-item-icon lgi-icon-bs"></span>
      <span class="list-group-item-text">
        <span>Bootstrap documentation: Badge</span>
        <span>Most of the details have been covered here</span>
      </span>
    </a>
    <a href="https://material.io/components/bottom-navigation#behavior" rel="external nofollow noopener" target="_blank" class="list-group-item list-group-item-action d-flex font-weight-bold">
    <span class="list-group-item-icon lgi-icon-md"></span>
    Material Design guidelines: Bottom navigation - Badges</a>
</div>

## Text with a badge

A badge can be appended to a text with 2 conditions:

1. Text is wrapped in a `<span class="position-relative">` element. This text container must be of `position: relative` for badge absolute positioning.
1. Badge is inserted within this text element.

{% capture example %}
<p class="typography-body-1">
  <span class="position-relative">Text with a badge
    <span class="badge badge-primary">4</span>
  </span>
</p>
{% endcapture %}
{% include example.html content=example %}

## Button with a badge

Just add your badge element beside button's text.

Badge can be left aligned with `.badge-before`.

{% capture example %}
<button type="button" class="btn btn-primary">
  Notifications
  <span class="badge badge-danger">8</span>
</button>

<button type="button" class="btn btn-primary ml-5">
  Action
  <span class="badge badge-secondary badge-before">2</span>
</button>
{% endcapture %}
{% include example.html content=example %}

## Icon with a badge

Add `.position-relative` class to your `<i>` or `<span>` element containing your icon (material icons, Fontawesome ...) and insert badge beside icon's name.

`.badge-before` class is still available.

{% capture example %}
<span class="material-icons position-relative">
  home
  <span class="badge badge-danger">15</span>
</span>

<span class="material-icons position-relative ml-5">
  home
  <span class="badge badge-danger badge-before">999</span>
</span>
{% endcapture %}
{% include example.html content=example %}
