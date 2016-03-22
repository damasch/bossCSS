---
layout: page
title: bossCSS - Example for a modified class
permalink: /examples/example_modified_class.html
---

If you declare a modifier for your module.
Rewrite every Property in a scope of the modifier.

```html
<div class="m-vcard m-vcard--private">
	<p class="m-vcard-name"></p>
	...
</div>
```

## PHP class definition:

```php
<?php
class vcard
{
	public $name = "...";
	public $position = "...";
	public $department = "...";
	public $email = "...";
	public $phone = "...";
	public $adress = "...";
	public $zip = "...";
	public $city = "...";

	public function __construct()
	{
	}

	// remember m-vcard--private
	public function mPrivateName() ...
	public function mPrivatePosition() ...
	public function mPrivateDepartment() ...


	public function mPrivateZipAndCity() ...
}
?>
```

## SCSS

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

	&--private &-name {...}
	&--private &-position {...}
	&--private &-department{...}

	&--private &-zip,
	&--private &-city
	{...}
}
```

## CSS

```css
.m-vacrad-name {...}
.m-vacrad-position {...}
.m-vacrad-department{...}
.m-vacrad-email{...}
.m-vacrad-phone{...}
.m-vacrad-adress{...}
.m-vacrad-zip{...}
.m-vacrad-city{...}

.m-vcard--private .m-vcard-name {...}
.m-vcard--private .m-vcard-position {...}
.m-vcard--private .m-vcard-department{...}

.m-vcard--private .m-vcard-zip,
.m-vcard--private .m-vcard-city
{...}

```


[Examples](example_list.html)