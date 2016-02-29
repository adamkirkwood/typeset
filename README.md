# Typeset, a simple typesetting mixin that uses Sass Maps

Setup just uses a nested Sass Map structure

~~~scss
$typesettings: (
  // Perfect Fourth @ 18px (1.125em)
  heading: (
    'h1': 2.369em,
    'h2': 1.777em,
    'h3': 1.333em,
    'h4': 1em,
    'h5': 0.75em
  ),
  ui: (
  	// ... snip ...
  )
);
~~~

Using `typeset` is simple:

~~~scss
h1 {
  font-size: typeset(heading, h1);
}
~~~