---
layout: page
title: Example for a static class
permalink: /examples/example_static_class.html
---

Fontdefinitions are a common problem for css development.
How many mixins and inlcudes are written for that simple stuff.
If we had an OOP structure, we would use a helper class.

## Markup

```html
<div class="l-headline__level1">Headline level 1<div>
<h1 class="l-headline__level1">Headline level 1<h1>
<h3 class="l-headline__level2">Headline hierarchie 3 looks like level 2</h3>
```

## PHP class definition:

```php
<?php
class headline
{
	public static function getLevel1() ...
	public static function getLevel2() ...
	public static function getLevel3() ...
	public static function getLevel4() ...
}
?>
```

## SCSS in a abstract version

```scss
.l-headline
{
	& ,
	&__level1 ,
	&__level2 ,
	&__level3 ,
	&__level4 { /* Common set up */ }

	&__level1 {...}

	&__level2 {...}
	
	&__level3 {...}
	
	&__level4 {...}
	
}
```


## CSS

```css
.l-headline ,
.l-headline__level1 ,
.l-headline__level2 ,
.l-headline__level3 ,
.l-headline__level4 { /* Common set up */ }

.l-headline__level1 {...}
.l-headline__level2 {...}
.l-headline__level3 {...}
.l-headline__level4 {...}
```

[Examples](example_list.html)
