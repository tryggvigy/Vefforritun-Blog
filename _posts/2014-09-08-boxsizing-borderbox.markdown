---
layout: post
title: "box-sizing: border-box"
date: "2014-09-08"
comments: True
---

## What is box-sizing?

> The "box model" in CSS works like this:
>
> width + padding + border = actual visible/rendered width of box
>
> height + padding + border = actual visible/rendered height of box
>
> <small>_Chris Coyier_</small> [http://css-tricks.com/box-sizing/](http://css-tricks.com/box-sizing/)

![http://www.geekchamp.com/upload/Tutorials/marginvspadding.png](http://www.geekchamp.com/upload/Tutorials/marginvspadding.png)

The box-sizing property is used to tell the browser what the sizing properties (width and height) should include. <br>
It's default value is box-sizing: content-box

The border-box value (as opposed to the content-box default) makes the final rendered box the declared width, and any border and padding cut inside the box.

## Using box-sizing: border-box

Here you can see the same code, with and without box-sizing: border-box;

### Without border-box
<p data-height="266" data-theme-id="8166" data-slug-hash="fJgjk" data-default-tab="result" data-user="tryggvigy" class='codepen'>See the Pen <a href='http://codepen.io/tryggvigy/pen/fJgjk/'>fJgjk</a> by Tryggvi Gylfason (<a href='http://codepen.io/tryggvigy'>@tryggvigy</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//codepen.io/assets/embed/ei.js"></script>

This is no good!

### With border-box
<p data-height="268" data-theme-id="8166" data-slug-hash="EjCty" data-default-tab="result" data-user="tryggvigy" class='codepen'>See the Pen <a href='http://codepen.io/tryggvigy/pen/EjCty/'>EjCty</a> by Tryggvi Gylfason (<a href='http://codepen.io/tryggvigy'>@tryggvigy</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//codepen.io/assets/embed/ei.js"></script>

Above you can see that no matter the padding I set, the border-width I use, the margin I set on the parent element, box1 will always be 50% of its parent width and box2 will always be 40% of the width.
Also they will always have 10% space between them.
