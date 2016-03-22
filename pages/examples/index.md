---
layout: page
title: Examples
permalink: /examples/index.html
---
## Introdution

A module has some diffrent properties, who will be displayed in a html Markup.
In this case you have an vcard.

V-Card properties:

- Name
- Persona
	- Position
	- Department
- Contact
	- Email
	- Phone
- Postal
	- Adress
	- Zip
	- City 
	- Country

### The bad way

The markup for these properteries could be developed maybe like this way.


```html
<div class="m-vcard">
	<p class="m-vcard-name"></p>
	<div class="m-vcard-persona">
		<p class="m-vcard-persona-position"></p>
		<p class="m-vcard-persona-department"></p>
	</div>
	<div class="m-vcard-contact">
		<p class="m-vcard-contact-email"></p>
		<p class="m-vcard-contact-phone"></p>
	</div>
	<div class="m-vcard-postal">
		<p class="m-vcard-postal-adress"></p>
		<span class="m-vcard-postal-zip"></span>
		<span class="m-vcard-postal-city"></span>
	</div>
</div>
```

## Let's think about classes

It's not nessesary to rebuild the dom structure.
Persona, Contact and Postal are wording groups for our definitions.
Think in OOP-Classes (in this case PHP).

If you write an vcard class in PHP ist looks like this.

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
}
```

## The better way

If you write your modules like classes in a oop class pattern you 
will understand the word for class="" in a html tag.

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


[Examples](example_list.html)



