# Components list

## `images`

Centers images and sets their width to 80% of the containing element.

## `paragraph`

Applies a serif font-face, justifies, and indents all paragraph elements.

## `skin-warning`

Creates a helper class for elements that should only be visible when work skins are disabled.

_Example:_

```html
<p class="skin-warning"><b>A/N:</b> This work relies on a skin to make it look better. Enable the skin by clicking here: <a href="?style=creator">[Enable work skin]</a></p>
```

## `texting`

Provides classes and structure for displaying text messaging. Currently looks like the Android Messages app, but more styles will be on the way.

_Example:_

```html
<!-- All text messages are contained in a div.texting-container -->
<div class="texting-container">
	<!-- Consecutive lines from one person are contained in a div with classes indicating side and color -->
	<div class="left red">
		<!-- A paragraph with the class 'name' will be used as a label for who's speaking - put it at the top -->
		<p class="name">Edgelord</p>
		<!-- Messages are plain paragraph elements -->
		<p>Hi, I'm an edgy edgelord.</p>
		<p>How are you?</p>
	</div>
</div>
```
