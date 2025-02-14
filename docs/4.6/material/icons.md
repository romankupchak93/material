---
layout: docs
title: Icons
description: Material takes advantage of the over 900 icons offered by the official icon set from Google.
group: material
redirect_from:
  - /docs/4.4/material/icons/
  - /docs/4.5/material/icons/
---

<div class="list-group">
  <a href="https://fonts.google.com/icons?selected=Material+Icons&icon.style=Outlined" rel="external nofollow noopener" target="_blank" class="list-group-item list-group-item-action d-flex font-weight-bold">
    <span class="list-group-item-icon lgi-icon-md"></span>
    Material Design Icons</a>
</div>

## Choose your icon set

*Daemonite Material Design for Bootstrap 4* is dependent of Material Design Icons and therefore requires at least this stylesheet declaration in your HTML header.

{% highlight html %}
<link href="{{ site.cdn.md_icon }}" rel="stylesheet" crossorigin>
{% endhighlight %}

For more creativity, it is compatible with all variants of Material Design Icons (**Filled, Outlined, Rounded, Two-Tone and Sharp versions**, declared in the same order below).

You can apply changes to your page immediately by modifying the stylesheet declaration according to the icon set you want (pick the one you want below).

{% highlight html %}
<link href="https://fonts.googleapis.com/css2?family=Material+Icons" rel="stylesheet" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Material+Icons+Outlined" rel="stylesheet" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Material+Icons+Round" rel="stylesheet" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Material+Icons+Two+Tone" rel="stylesheet" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Material+Icons+Sharp" rel="stylesheet" crossorigin>
{% endhighlight %}

You can even mix multiple icons sets within your page with a combined stylesheet declaration like this (i.e. Baseline and Outlined versions).

{% highlight html %}
<link href="https://fonts.googleapis.com/css2?family=Material+Icons&family=Material+Icons+Outlined" rel="stylesheet" crossorigin>
{% endhighlight %}

## HTML markup

Then, it is easy to incorporate icons into your web page. You can browse the icon set and copy-paste the HTML markup from the [Material icons library](https://material.io/resources/icons/).

Here is a small example:

{% capture example %}
<span class="material-icons">face</span>
{% endcapture %}
{% include example.html content=example %}

**NB.** In order to allow you to switch fast from one icon set to another, Daemonite Material Design promotes the usage of the default HTML markup using `<span class="material-icons">...</span>` (and avoid specific ones like `<span class="material-icons-outlined">...</span>`).

Hence, you can swith from one icon set to another without rewriting all your icon tags.

### HTML markup with different icon styles

In the case you want to use 2 different Materials Icons sets (i.e. Baseline and Outlined icons) on a page, you will need to specify `<span class="material-icons-outlined">...</span>` for the icons that will have to be in an Outlined style.

For a **Sharp** + **Round** combination, you must declare icons with both `<span class="material-icons-sharp">...</span>` and `<span class="material-icons-round">...</span>` tags.

In case you want to switch to a single Material Icons set, as seen above, you don't have to change all your icon HTML markup, they will all be set to your current declared Material Icons set.
In fact, all icons declared with `.material-icons*` will style according to the active font stylesheet.

## Browser support

**NB. For browsers that do not [support ligatures (IE11)](https://caniuse.com/kerning-pairs-ligatures), fall back to specifying the icons using numeric character references like the example below:**

{% capture example %}
<span class="material-icons">&#xE87C;</span>
{% endcapture %}
{% include example.html content=example %}

For all available icons, [see Material icons library](https://material.io/resources/icons/).
