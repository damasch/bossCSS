---
layout: page
title: bossCSS - Example for a default class
permalink: /examples/example_default_class.html
---

Similar to the written Markup remove the parent grouping names.

```html
<div class="m-vcard">
	<p class="m-vcard-name"></p>
	<div class="m-vcard-persona">
		<p class="m-vcard-position"></p>
		<p class="m-vcard-department"></p>
	</div>
	<div class="m-vcard-contact">
		<p class="m-vcard-email"></p>
		<p class="m-vcard-phone"></p>
	</div>
	<div class="m-vcard-postal">
		<p class="m-vcard-adress"></p>
		<span class="m-vcard-zip"></span>
		<span class="m-vcard-city"></span>
	</div>
</div>
```

## SCSS
Write down the scss file

```scss
.m-vcard
{
	/* eg Constructor */
	...
	&-name {...}
	&-position {...}
	&-department{...}
	&-email{...}
	&-phone{...}
	&-adress{...}
	&-zip{...}
	&-city{...}
}
```

## CSS
After the redering of sass, the code should look like

```css
.m-vacrad-name {...}
.m-vacrad-position {...}
.m-vacrad-department{...}
.m-vacrad-email{...}
.m-vacrad-phone{...}
.m-vacrad-adress{...}
.m-vacrad-zip{...}
.m-vacrad-city{...}
```


[Examples](example_list.html)