---
layout: docs
title: Placeholders
description: Use loading placeholders for your components or pages to indicate something may still be loading.
group: components
toc: true
added: "5.1"
---

## About

Placeholders can be used to enhance the experience of your application.

## Example

<div class="bd-example bd-example-placeholder-cards d-flex justify-content-around">
<div class="card">
  {{< placeholder width="100%" height="180" class="card-img-top" text="false" background="#20c997" >}}
  <div class="card-body">
    <h5 class="card-title">Card title</h5>
    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>

<div class="card" aria-hidden="true">
  {{< placeholder width="100%" height="180" class="card-img-top" text="false" >}}
  <div class="card-body">
    <div class="h5 card-title placeholder-glow">
      <span class="placeholder col-6"></span>
    </div>
    <p class="card-text placeholder-glow">
      <span class="placeholder col-7"></span>
      <span class="placeholder col-4"></span>
      <span class="placeholder col-4"></span>
      <span class="placeholder col-6"></span>
      <span class="placeholder col-8"></span>
    </p>
    <a class="btn btn-primary disabled placeholder col-6"></a>
  </div>
</div>
</div>

## How it works

<div class="bd-example-snippet bd-code-snippet p-1"><div class="bd-example m-1  border-0">

<p aria-hidden="true">
  <span class="placeholder col-6"></span>
</p>

<a class="btn btn-primary disabled placeholder col-4"></a>

</div></div>

### Width

<div class="bd-example-snippet bd-code-snippet p-1"><div class="bd-example m-1  border-0">
<span class="placeholder col-6"></span>
<span class="placeholder w-75"></span>
<span class="placeholder" style="width: 25%;"></span>

</div></div>

### Color

<div class="bd-example-snippet bd-code-snippet p-1"><div class="bd-example m-1  border-0">
<span class="placeholder col-12"></span>
{{< placeholders.inline >}}
{{- range (index $.Site.Data "theme-colors") }}
<span class="placeholder col-12 bg-{{ .name }}"></span>
{{- end -}}
{{< /placeholders.inline >}}

</div></div>

### Sizing

<div class="bd-example-snippet bd-code-snippet p-1"><div class="bd-example m-1  border-0">
<span class="placeholder col-12 placeholder-lg"></span>
<span class="placeholder col-12"></span>
<span class="placeholder col-12 placeholder-sm"></span>
<span class="placeholder col-12 placeholder-xs"></span>

</div></div>

### Animation

<div class="bd-example-snippet bd-code-snippet p-1"><div class="bd-example m-1  border-0">

<p class="placeholder-glow">
  <span class="placeholder col-12"></span>
</p>

<p class="placeholder-wave">
  <span class="placeholder col-12"></span>
</p>
</div></div>
