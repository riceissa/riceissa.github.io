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

This page is also an example of using Liquid to reduce redundancy.
It seems to mostly work, but some outputs seem to be different.
See [here](#diff-output) for an example.
See [the source](https://raw.githubusercontent.com/riceissa/riceissa.github.io/master/math/math-test.md) for more.

If you are wondering which inputs work the best, see [Backtick:Single backslash parenthesis](#bsbp) and [Backtick:Single backslash bracket](#bsbb).
For inputting these, see [here](/computing/jekyll.html#examples).

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

<h3 id="bsbp">Single backslash parenthesis</h3>

`\({% include integral-test.html %}\)`

`\({% include cross-product-test.html %}\)`

<h3 id="bsbb">Single backslash bracket</h3>

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

<h3 id="diff-output">Single backslash parenthesis</h3>

    \({% include integral-test.html %}\)

<!-- -->

    \(F(a,b) = \int_a^b f(x)\, dx > 1\)

<!-- -->

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
