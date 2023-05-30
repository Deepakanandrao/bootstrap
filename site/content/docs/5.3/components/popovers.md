---
layout: docs
title: Popovers
description: Documentation and examples for adding Bootstrap popovers, like those found in iOS, to any element on your site.
group: components
toc: true
---

## Examples

<div stackblitz_add_js="true"><div class="bd-example-snippet bd-code-snippet p-1">
<button type="button" class="btn btn-lg btn-danger" data-bs-toggle="popover" data-bs-title="Popover title" data-bs-content="And here's some amazing content. It's very engaging. Right?">Click to toggle popover</button>

</div></div>

### Four directions

<div stackblitz_add_js="true"><div class="bd-example-snippet bd-code-snippet p-1">
<button type="button" class="btn btn-secondary" data-bs-container="body" data-bs-toggle="popover" data-bs-placement="top" data-bs-content="Top popover">
Popover on top
</button>
<button type="button" class="btn btn-secondary" data-bs-container="body" data-bs-toggle="popover" data-bs-placement="right" data-bs-content="Right popover">
Popover on right
</button>
<button type="button" class="btn btn-secondary" data-bs-container="body" data-bs-toggle="popover" data-bs-placement="bottom" data-bs-content="Bottom popover">
Popover on bottom
</button>
<button type="button" class="btn btn-secondary" data-bs-container="body" data-bs-toggle="popover" data-bs-placement="left" data-bs-content="Left popover">
Popover on left
</button>

</div></div>

<div class="custom-popover-demo" stackblitz_add_js="true"><div class="bd-example-snippet bd-code-snippet p-1">
<button type="button" class="btn btn-secondary"
        data-bs-toggle="popover" data-bs-placement="right"
        data-bs-custom-class="custom-popover"
        data-bs-title="Custom popover"
        data-bs-content="This popover is themed via CSS variables.">
Custom popover
</button>

</div></div>

### Dismiss on next click

<div stackblitz_add_js="true"><div class="bd-example-snippet bd-code-snippet p-1">
<a tabindex="0" class="btn btn-lg btn-danger" role="button" data-bs-toggle="popover" data-bs-trigger="focus" data-bs-title="Dismissible popover" data-bs-content="And here's some amazing content. It's very engaging. Right?">Dismissible popover</a>

</div></div>

### Disabled elements

<div stackblitz_add_js="true"><div class="bd-example-snippet bd-code-snippet p-1">
<span class="d-inline-block" tabindex="0" data-bs-toggle="popover" data-bs-trigger="hover focus" data-bs-content="Disabled popover">
<button class="btn btn-primary" type="button" disabled>Disabled button</button>
</span>

</div></div>
