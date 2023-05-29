---
layout: docs
title: Buttons
description: Use Bootstrap's custom button styles for actions in forms, dialogs, and more with support for multiple sizes, states, and more.
group: components
toc: true
---

## Buttons

Bootstrap includes several button variants, each serving its own semantic purpose, with a few extras thrown in for more control.
e.g. ` .btn .btn-primary`

<div class="bd-example-snippet bd-code-snippet p-1"><div class="bd-example m-1  border-0">
{{< buttons.inline >}}
{{- range (index $.Site.Data "theme-colors") }}
<button type="button" class="btn btn-{{ .name }}">{{ .name | title }}</button>
{{- end -}}
{{< /buttons.inline >}}

<button type="button" class="btn btn-link">Link</button>

</div></div>

## Outline buttons

In need of a button, but not the hefty background colors they bring? Replace the default modifier classes with the `.btn-outline-*` ones to remove all background images and colors on any button.

<div class="bd-example-snippet bd-code-snippet p-1"><div class="bd-example m-1  border-0">
{{< buttons.inline >}}
{{- range (index $.Site.Data "theme-colors") }}
<button type="button" class="btn btn-outline-{{ .name }}">{{ .name | title }}</button>
{{- end -}}
{{< /buttons.inline >}}

</div></div>

## Sizes

Fancy larger or smaller buttons? Add `.btn-lg` or `.btn-sm` for additional sizes.

<div class="bd-example-snippet bd-code-snippet p-1"><div class="bd-example m-1  border-0">
<button type="button" class="btn btn-primary btn-lg">Large button</button>
<button type="button" class="btn btn-secondary btn-lg">Large button</button>

</div></div>

<div class="bd-example-snippet bd-code-snippet p-1"><div class="bd-example m-1  border-0">
<button type="button" class="btn btn-primary btn-sm">Small button</button>
<button type="button" class="btn btn-secondary btn-sm">Small button</button>

</div></div>

You can even roll your own custom sizing with CSS variables:

<div class="bd-example-snippet bd-code-snippet p-1"><div class="bd-example m-1  border-0">
<button type="button" class="btn btn-primary"
        style="--bs-btn-padding-y: .25rem; --bs-btn-padding-x: .5rem; --bs-btn-font-size: .75rem;">
Custom button
</button>

</div></div>

## Disabled state

Make buttons look inactive by adding the `disabled` boolean attribute to any `<button>` element. Disabled buttons have `pointer-events: none` applied to, preventing hover and active states from triggering.

<div class="bd-example-snippet bd-code-snippet p-1"><div class="bd-example m-1  border-0">
<button type="button" class="btn btn-primary" disabled>Primary button</button>
<button type="button" class="btn btn-secondary" disabled>Button</button>
<button type="button" class="btn btn-outline-primary" disabled>Primary button</button>
<button type="button" class="btn btn-outline-secondary" disabled>Button</button>

</div></div>
