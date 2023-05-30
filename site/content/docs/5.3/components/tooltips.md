---
layout: docs
title: Tooltips
description: Documentation and examples for adding custom Bootstrap tooltips with CSS and JavaScript using CSS3 for animations and data-bs-attributes for local title storage.
group: components
toc: true
---

Tooltips on links

Hover over the links below to see tooltips:

<div class="tooltip-demo" stackblitz_add_js="true"><div class="bd-example-snippet bd-code-snippet p-1">

<p class="muted">Placeholder text to demonstrate some <a href="#" data-bs-toggle="tooltip" data-bs-title="Default tooltip">inline links</a> with tooltips. This is now just filler, no killer. Content placed here just to mimic the presence of <a href="#" data-bs-toggle="tooltip" data-bs-title="Another tooltip">real text</a>. And all that just to give you an idea of how tooltips would look when used in real-world situations. So hopefully you've now seen how <a href="#" data-bs-toggle="tooltip" data-bs-title="Another one here too">these tooltips on links</a> can work in practice, once you use them on <a href="#" data-bs-toggle="tooltip" data-bs-title="The last tip!">your own</a> site or project.</p>
</div></div>

Custom tooltips

<div class="tooltip-demo" stackblitz_add_js="true"><div class="bd-example-snippet bd-code-snippet p-1">
<button type="button" class="btn btn-secondary"
        data-bs-toggle="tooltip" data-bs-placement="top"
        data-bs-custom-class="custom-tooltip"
        data-bs-title="This top tooltip is themed via CSS variables.">
Custom tooltip
</button>

</div></div>

Directions

<div class="bd-example tooltip-demo">
  <div class="bd-example-tooltips">
    <button type="button" class="btn btn-secondary" data-bs-toggle="tooltip" data-bs-placement="top" data-bs-title="Tooltip on top">Tooltip on top</button>
    <button type="button" class="btn btn-secondary" data-bs-toggle="tooltip" data-bs-placement="right" data-bs-title="Tooltip on right">Tooltip on right</button>
    <button type="button" class="btn btn-secondary" data-bs-toggle="tooltip" data-bs-placement="bottom" data-bs-title="Tooltip on bottom">Tooltip on bottom</button>
    <button type="button" class="btn btn-secondary" data-bs-toggle="tooltip" data-bs-placement="left" data-bs-title="Tooltip on left">Tooltip on left</button>
    <button type="button" class="btn btn-secondary" data-bs-toggle="tooltip" data-bs-html="true" data-bs-title="<em>Tooltip</em> <u>with</u> <b>HTML</b>">Tooltip with HTML</button>
  </div>
</div>

<div class="bd-example tooltip-demo">
  <a href="#" class="d-inline-block" data-bs-toggle="tooltip" data-bs-title="Default tooltip">
    <svg xmlns="http://www.w3.org/2000/svg" width="50" height="50" viewBox="0 0 100 100">
      <rect width="100%" height="100%" fill="#563d7c"/>
      <circle cx="50" cy="50" r="30" fill="#007bff"/>
    </svg>
  </a>
</div>
