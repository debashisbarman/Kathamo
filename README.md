Kathamo CSS Framework
=====================

Kathamo is a minimalist CSS framework that can help you rapidly develop sites that look beautiful at any size, be it a 17" laptop screen or an iPhone.
>Kathamo is an Assamese word, literary meaning "structure" or "frame"; thus the name itself suggests a framework. 

Kathamo is based on the following principles:

**Responsive Grid:** Kathamo has a familiar, lightweight 1024 grid as its base, but elegantly scales down to downsized browser windows, tablets, mobile phones (in landscape and portrait).

**Faster Development:** Kathamo is a tool for rapid development with easy CSS and a well-structured Grid.

**Minimal UI:** Kathamo is not a UI framework. It's a development kit that provides the most basic styles as a foundation, but is ready to adopt whatever your design or style is.

##Development
Kathamo is developed by [Debashis Barman](http://www.debashisbarman.in). Kathamo 2.0.0 is currently the stable version. This version of Kathamo includes:

<ul>
<li>Base CSS file for basic styles as a foundation.</li>
<li>A 1024 Grid system with responsive elements.</li>
</ul>

##License
All the files in this repository are [MIT](http://opensource.org/licenses/MIT) licensed.

#Documentation

Kathamo 2.0.0 (Stable) has a few easy ways to quickly get started, each one appealing to a different skill level and use case. Read through to see what suits your particular needs.

## Basic Template

Start with the below to begin working with a minimal Kathamo document.

```
<!DOCTYPE html>
<html lang="en">

<head>
	<meta charset="utf-8">
	<meta http-equiv="X-UA-Compatible" content="IE=edge">
	<meta name="viewport" content="width=device-width, initial-scale=1">
	<title></title>

	<!-- Kathamo -->
	<link href="kathamo/kathamo.css" rel="stylesheet">
</head>

<body></body>

</html>
```

##Grid System

Kathamo includes a responsive, mobile first fluid grid system that appropriately scales up to 12 columns as the device or viewport size increases. In Kathamo, all the columns must be wrapped inside a `.row` and all the rows must be wrapped inside a `.container`. The column classes follows the pattern `col-*-**` where the `*` indicates `lg`, `md` and `sm` and `**` indicates the size of the column, ranging from 1 to 11.

```
<!-- `.container` is the main wrapper for the grid. -->
<div class="container">

	<!-- All columns must be wrapped in a `.row`. -->
	<div class="row">

	<!-- Grid columns are created by specifying the number of 12 available columns you wish to span. -->
	<div class="col-lg-3 col-md-5 col-sm-12"></div>
	<div class="col-lg-9 col-md-7 col-sm-12"></div>

	</div>

</div>
```

##Typography

The base typeface of Kathamo is [Raleway](http://www.google.com/fonts/specimen/Raleway) served by Google, set at `font-size: 15px` over `line-height: 1.618` with `letter-spacing: 0.618px` and `font-weight: 300`.

```
<!-- Standard Headings -->
<h1>Kathamo <small>Framework</small></h1>
<h2>Kathamo <small>Framwork</small></h2>
<h3>Kathamo <small>Framwork</small></h3>
<h4>Kathamo <small>Framwork</small></h4>
<h5>Kathamo <small>Framwork</small></h5>
<h6>Kathamo <small>Framwork</small></h6>

<!-- Body Text -->
<p>Kathamo <small>Framework</small></p>

<!-- Other styled text tags -->
<strong>Bolded</strong>
<em>Italicized</em>
<a>Colored</a>
<u>Underlined</u>
```

##List

Basic `<ol>` and `<ul>` are unstyled. Use `li-unstyled`, `li-inline`, `li-circle`, `li-square`, `li-disc`, `<dl>` to add styling.

```
<!-- Ordered List -->
<ol>
<li>Item 1</li>
<li>Item 2</li>
<li>Item 3</li>
<li>Item 4</li>
</ol>

<!-- Unstyled List -->
<ol class="li-unstyled">
<li>Item 1</li>
<li>Item 2</li>
<li>Item 3</li>
<li>Item 4</li>
</ol>

<!-- Inline List -->
<ol class="li-inline">
<li>Item 1</li>
<li>Item 2</li>
<li>Item 3</li>
<li>Item 4</li>
</ol>

<!-- Unorderd List -->
<ul class="li-circle">
<li>Item 1</li>
<li> Item 3
<ul class="li-square">
<li>Item 1</li>
<li>Item 2
<ul class="li-disc">
<li>Item 1</li>
<li>Item 2</li>
</ul>
</li>
</ul>
</li>
<li>Item 3</li>
</ul>

<!-- Data List -->
<dl>
<dt>Title 1</dt>
<dd>Item 1</dd>
<dt>Title 2</dt>
<dd>Item 2</dd>
</dl>

<!-- Inline Data List -->
<dl class="li-inline">
<dt>Inline Data List</dt>
<dd>Item 1</dd>
<dd>Item 2</dd>
<dd>Item 3</dd>
<dd>Item 4</dd>
</dl>
```


##Blockquote

Use `<blockquote>` for quoting blocks of content from another source within your document.

```
<blockquote>
Kathamo is an Assamese word, literary meaning "structure" or "frame"; thus the name itself suggests a framework.
<cite>Debashis Barman, Kathamo Creator</cite>
</blockquote>
```

##Code

Use `<code>` for wrapping inline snippets of code and `<pre>` for multiple lines of code.

```
<!-- For inline snippets of code. -->
<p>Use <code>&lt;code&gt;</code> for wrapping inline snippets of code.</p>

<!-- For multiple lines of code. -->
<pre>
&lt;link href="kathamo/kathamo.css" rel="stylesheet" /&gt;
</pre>
```

##Image

All `<img>` in Kathamo are responsive. Kathamo provides two standard classes `img-circle` and `img-border`. Also use `left-text-wrap` or `right-text-wrap` to the `<img>` for wrapping text around a image.

##Table

Use `.table` to any `<table>` for adding basic styling to it.

```
<table class="table">
  ...
</table>
```

###Bordered Table

Use `.table-bordered` for borders on all sides of the table and cells.

```
<table class="table table-bordered">
  ...
</table>
```

###Borderless Table

Use `.table-no-border` to remove borders on all sides of the table and cells.

```
<table class="table table-no-border">
  ...
</table>
```

###Striped Rows

Use `.table-striped` to add zebra-striping to any table row within the `<tbody>`.

```
<table class="table table-striped">
  ...
</table>
```

###Responsive Table

Wrap `.table` in `.table-responsive` to make responsive table.

```
<div class="table-responsive">
<table class="table">
  ...
</table>
</div>
```

##Form

Use standard HTML tags for `<label>`, `<input>`, `<select>` and `<textarea>`. Kathamo provides custom style for different input types viz. text, password, email, search, checkbox and radio.

```
<form  ...  >
	<div class="col-lg-6 col-md-6 col-sm-12">
	<label>Your email</label>
	<input type="text" name="email" placeholder="me@example.com"/>
	</div>

	<div class="col-lg-6 col-md-6 col-sm-12">
	<label>You're from</label>
	<select class="ui-full-width">
	<option>Country</option>
	<option name="country" value="Option 1">India</option>
	<option name="country" value="Option 2">Outside India</option>
	</select>
	</div>

	<div class="col-lg-12 col-md-12 col-sm-12">
	<label>Message</label>
	<textarea name="message" placeholder="Hi! Deb..."></textarea>
	</div>

	<div class="col-lg-12 col-md-12 col-sm-12">
	<input type="checkbox" name="copy-to-yourself">Send a copy to yourself.
	</div>

	<div class="col-lg-12 col-md-12 col-sm-12">
	<input type="submit" class="btn btn-success" value="Submit">
	<input type="reset" class="btn btn-danger" value="Clear">
	</div>
</form>
```

##Button

Use `.btn` to any standard HTML button with `btn-default`, `btn-success`, `btn-danger` to add styling to it. Kathamo also supports anchor buttons.

```
<!-- Buttons -->
<button type="button" class="btn btn-default">Default</button>
<button type="submit" class="btn btn-success">Success</button>
<button type="reset" class="btn btn-danger">Danger</button>

<!-- Input Types -->
<input type="button" class="btn btn-default" value="Default">
<input type="submit" class="btn btn-success" value="Success">
<input type="reset" class="btn btn-danger" value="Danger">

<!-- Anchor Buttons -->
<a type="button" class="btn btn-default" href="">Default</a>
<a type="button" class="btn btn-success" href="">Success</a>
<a type="button" class="btn btn-danger" href="">Danger</a>
```

##Alerts & Panel

Provide contextual feedback messages for typical user actions with the handful of available and flexible alert messages and panel.
