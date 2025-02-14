---
layout: docs
title: Progress
description: Progress indicators express an unspecified wait time or display the length of a process.
group: material
redirect_from:
  - /docs/4.4/material/progress/
  - /docs/4.5/material/progress/
toc: true
---

<div class="list-group my-2 my-lg-5">
    <a href="{{ site.baseurl }}/docs/{{ site.docs_version }}/components/progress/" target="_blank" class="list-group-item list-group-item-action d-flex list-group-item-two-line font-weight-bold">
      <span class="list-group-item-icon lgi-icon-bs"></span>
      <span class="list-group-item-text">
        <span>Bootstrap documentation: Progress</span>
        <span>Most of the details have been covered here</span>
      </span>
    </a>
    <a href="https://material.io/components/progress-indicators" rel="external nofollow noopener" target="_blank" class="list-group-item list-group-item-action d-flex font-weight-bold">
      <span class="list-group-item-icon lgi-icon-md"></span>
      Material Design guidelines: Progress indicators</a>
    <a href="https://material-components.github.io/material-components-web-catalog/#/component/linear-progress-indicator" rel="external nofollow noopener" target="_blank" class="list-group-item list-group-item-action d-flex font-weight-bold">
      <span class="list-group-item-icon lgi-icon-mdc"></span>
      Material Components for the web: Linear Progress Indicator</a>
</div>

Progress indicators inform users about the status of ongoing processes, such as loading an app, submitting a form, or saving updates. They communicate an app’s state and indicate available actions, such as whether users can navigate away from the current screen.

**Progress as a group**
When displaying progress for a sequence of processes, indicate overall progress rather than the progress of each activity.

## Circular progress

Circular progress is built with a group of HTML elements, below is a detailed example.

{% capture example %}
<div class="progress-circular">
  <div class="progress-circular-wrapper">
    <div class="progress-circular-inner">
      <div class="progress-circular-left">
        <div class="progress-circular-spinner"></div>
      </div>
      <div class="progress-circular-gap"></div>
      <div class="progress-circular-right">
        <div class="progress-circular-spinner"></div>
      </div>
    </div>
  </div>
</div>
{% endcapture %}
{% include example.html content=example %}

Add additional color classes (e.g. brand colors: <code>-primary</code>, <code>-secondary</code>, or helper colors: <code>-danger</code>, <code>-info</code>, <code>-success</code>, <code>-warning</code>) to change the appearance of individual circular progress.

{% capture example %}
<div class="progress-circular progress-circular-primary">
  <div class="progress-circular-wrapper">
    <div class="progress-circular-inner">
      <div class="progress-circular-left">
        <div class="progress-circular-spinner"></div>
      </div>
      <div class="progress-circular-gap"></div>
      <div class="progress-circular-right">
        <div class="progress-circular-spinner"></div>
      </div>
    </div>
  </div>
</div>
{% endcapture %}
{% include example.html content=example %}

## Linear progress

**Most of the details about linear progress have been covered in Components/Progress documentation. Read more about [Progress component]({{ site.baseurl }}/docs/{{ site.docs_version }}/components/progress/).**

### Indeterminate linear progress

When indicators are indeterminate they request that the user wait while something finishes when it’s not necessary to indicate how long it will take.

Create an indeterminate linear progress by adding `.progress-bar-indeterminate` class.

{% capture example %}
<div class="progress">
  <div class="progress-bar progress-bar-indeterminate" role="progressbar"></div>
</div>
{% endcapture %}
{% include example.html content=example %}
