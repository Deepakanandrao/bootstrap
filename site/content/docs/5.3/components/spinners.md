---
layout: docs
title: Spinners
description: Indicate the loading state of a component or page with Bootstrap spinners, built entirely with HTML, CSS, and no JavaScript.
group: components
toc: true
---

## Spinners

<div class="bd-example-snippet bd-code-snippet p-1"><div class="bd-example m-1  border-0">

<div class="spinner-border" role="status">
  <span class="visually-hidden">Loading...</span>
</div>
</div></div>

Colors

<div class="bd-example-snippet bd-code-snippet p-1"><div class="bd-example m-1  border-0">
{{< spinner.inline >}}
{{- range (index $.Site.Data "theme-colors") }}

<div class="spinner-border text-{{ .name }}" role="status">
  <span class="visually-hidden">Loading...</span>
</div>
{{- end -}}
{{< /spinner.inline >}}
</div></div>

Growing spinner

<div class="bd-example-snippet bd-code-snippet p-1"><div class="bd-example m-1  border-0">

<div class="spinner-grow" role="status">
  <span class="visually-hidden">Loading...</span>
</div>
</div></div>

<div class="bd-example-snippet bd-code-snippet p-1"><div class="bd-example m-1  border-0">
{{< spinner.inline >}}
{{- range (index $.Site.Data "theme-colors") }}

<div class="spinner-grow text-{{ .name }}" role="status">
  <span class="visually-hidden">Loading...</span>
</div>
{{- end -}}
{{< /spinner.inline >}}
</div></div>

Buttons

<div class="bd-example-snippet bd-code-snippet p-1"><div class="bd-example m-1  border-0">
<button class="btn btn-primary" type="button" disabled>
<span class="spinner-border spinner-border-sm" role="status" aria-hidden="true"></span>
<span class="visually-hidden">Loading...</span>
</button>
<button class="btn btn-primary" type="button" disabled>
<span class="spinner-border spinner-border-sm" role="status" aria-hidden="true"></span>
Loading...
</button>

</div></div>

<div class="bd-example-snippet bd-code-snippet p-1"><div class="bd-example m-1  border-0">
<button class="btn btn-primary" type="button" disabled>
<span class="spinner-grow spinner-grow-sm" role="status" aria-hidden="true"></span>
<span class="visually-hidden">Loading...</span>
</button>
<button class="btn btn-primary" type="button" disabled>
<span class="spinner-grow spinner-grow-sm" role="status" aria-hidden="true"></span>
Loading...
</button>

</div></div>
