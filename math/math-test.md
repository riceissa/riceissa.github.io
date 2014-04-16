---
layout: default
title: Testing Jekyll and Mathjax
comments: "no"
math: "yes"
---

So what works?
Below we check both

{% highlight tex %}
{% include integral-test.html %}
{% endhighlight %}

(to see if simple equations work) and

{% highlight tex %}
{% include cross-product-test.html %}
{% endhighlight %}

(to see if more complicated equations work, especially those containing a double backslash).

[This page is also an example of using Liquid to reduce redundancy. See [the source](https://raw.githubusercontent.com/riceissa/riceissa.github.io/master/math/math-test.md) for more.]

## Standard

### Single dollar

${% include integral-test.html %}$

${% include cross-product-test.html %}$

### Double dollar

$${% include integral-test.html %}$$

$${% include cross-product-test.html %}$$

### Single backslash parenthesis

\({% include integral-test.html %}\)

\({% include cross-product-test.html %}\)

### Single backslash bracket

\[{% include integral-test.html %}\]

\[{% include cross-product-test.html %}\]

### Double backslash parenthesis

\\({% include integral-test.html %}\\)

\\({% include cross-product-test.html %}\\)

### Double backslash bracket

\\[{% include integral-test.html %}\\]

\\[{% include cross-product-test.html %}\\]

##Backtick

### Single dollar

`${% include integral-test.html %}$`

`${% include cross-product-test.html %}$`

### Double dollar

`$${% include integral-test.html %}$$`

`$${% include cross-product-test.html %}$$`

### Single backslash parenthesis

`\({% include integral-test.html %}\)`

`\({% include cross-product-test.html %}\)`

### Single backslash bracket

`\[{% include integral-test.html %}\]`

`\[{% include cross-product-test.html %}\]`

### Double backslash parenthesis

`\\({% include integral-test.html %}\\)`

`\\({% include cross-product-test.html %}\\)`

### Double backslash bracket

`\\[{% include integral-test.html %}\\]`

`\\[{% include cross-product-test.html %}\\]`

## Fourspace

### Single dollar

    ${% include integral-test.html %}$

    ${% include cross-product-test.html %}$

### Double dollar

    $${% include integral-test.html %}$$

    $${% include cross-product-test.html %}$$

### Single backslash parenthesis

    \({% include integral-test.html %}\)

    \({% include cross-product-test.html %}\)

### Single backslash bracket

    \[{% include integral-test.html %}\]

    \[{% include cross-product-test.html %}\]

### Double backslash parenthesis

    \\({% include integral-test.html %}\\)

    \\({% include cross-product-test.html %}\\)

### Double backslash bracket

    \\[{% include integral-test.html %}\\]

    \\[{% include cross-product-test.html %}\\]

## Code

### Single dollar

<code>${% include integral-test.html %}$</code>

<code>${% include cross-product-test.html %}$</code>

### Double dollar

<code>$${% include integral-test.html %}$$</code>

<code>$${% include cross-product-test.html %}$$</code>

### Single backslash parenthesis

<code>\({% include integral-test.html %}\)</code>

<code>\({% include cross-product-test.html %}\)</code>

### Single backslash bracket

<code>\[{% include integral-test.html %}\]</code>

<code>\[{% include cross-product-test.html %}\]</code>

### Double backslash parenthesis

<code>\\({% include integral-test.html %}\\)</code>

<code>\\({% include cross-product-test.html %}\\)</code>

### Double backslash bracket

<code>\\[{% include integral-test.html %}\\]</code>

<code>\\[{% include cross-product-test.html %}\\]</code>

## Code Pre

### Single dollar

<code><pre>${% include integral-test.html %}$</pre></code>

<code><pre>${% include cross-product-test.html %}$</pre></code>

### Double dollar

<code><pre>$${% include integral-test.html %}$$</pre></code>

<code><pre>$${% include cross-product-test.html %}$$</pre></code>

### Single backslash parenthesis

<code><pre>\({% include integral-test.html %}\)</pre></code>

<code><pre>\({% include cross-product-test.html %}\)</pre></code>

### Single backslash bracket

<code><pre>\[{% include integral-test.html %}\]</pre></code>

<code><pre>\[{% include cross-product-test.html %}\]</pre></code>

### Double backslash parenthesis

<code><pre>\\({% include integral-test.html %}\\)</pre></code>

<code><pre>\\({% include cross-product-test.html %}\\)</pre></code>

### Double backslash bracket

<code><pre>\\[{% include integral-test.html %}\\]</pre></code>

<code><pre>\\[{% include cross-product-test.html %}\\]</pre></code>

    \(\sin (a+b) = \sin a\cos b x_i + \cos a\sin b ab\)
