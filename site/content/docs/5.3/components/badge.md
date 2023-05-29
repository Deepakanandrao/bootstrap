---
layout: docs
title: Badges
description: Documentation and examples for badges, our small count and labeling component.
group: components
toc: true
---

## Examples

Badges scale to match the size of the immediate parent element by using relative font sizing and `em` units. As of v5, badges no longer have focus or hover styles for links.

### Headings

<div class="bd-example-snippet bd-code-snippet p-1"><div class="bd-example m-1  border-0">

<h1>Example heading <span class="badge bg-secondary">New</span></h1>
<h2>Example heading <span class="badge bg-secondary">New</span></h2>
<h3>Example heading <span class="badge bg-secondary">New</span></h3>
<h4>Example heading <span class="badge bg-secondary">New</span></h4>
<h5>Example heading <span class="badge bg-secondary">New</span></h5>
<h6>Example heading <span class="badge bg-secondary">New</span></h6>
</div></div>

### Buttons

Badges can be used as part of links or buttons to provide a counter.

<div class="bd-example-snippet bd-code-snippet p-1"><div class="bd-example m-1  border-0">
<button type="button" class="btn btn-primary">
Notifications <span class="badge text-bg-secondary">4</span>
</button>

</div></div>

### Positioned

Use utilities to modify a `.badge` and position it in the corner of a link or button.

<div class="bd-example-snippet bd-code-snippet p-1"><div class="bd-example m-1  border-0">
<button type="button" class="btn btn-primary position-relative">
Inbox
<span class="position-absolute top-0 start-100 translate-middle badge rounded-pill bg-danger">
99+
<span class="visually-hidden">unread messages</span>
</span>
</button>

</div></div>

You can also replace the `.badge` class with a few more utilities without a count for a more generic indicator.

<div class="bd-example-snippet bd-code-snippet p-1"><div class="bd-example m-1  border-0">
<button type="button" class="btn btn-primary position-relative">
Profile
<span class="position-absolute top-0 start-100 translate-middle p-2 bg-danger border border-light rounded-circle">
<span class="visually-hidden">New alerts</span>
</span>
</button>

</div></div>

## Background colors

<div class="bd-example-snippet bd-code-snippet p-1"><div class="bd-example m-1  border-0">
{{< badge.inline >}}
{{- range (index $.Site.Data "theme-colors") }}
<span class="badge text-bg-{{ .name }}">{{ .name | title }}</span>{{- end -}}
{{< /badge.inline >}}

</div></div>

## Pill badges

Use the `.rounded-pill` utility class to make badges more rounded with a larger `border-radius`.

<div class="bd-example-snippet bd-code-snippet p-1"><div class="bd-example m-1  border-0">
{{< badge.inline >}}
{{- range (index $.Site.Data "theme-colors") }}
<span class="badge rounded-pill text-bg-{{ .name }}">{{ .name | title }}</span>{{- end -}}
{{< /badge.inline >}}

</div></div>
