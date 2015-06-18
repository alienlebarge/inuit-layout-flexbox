# inuit-flexbox

A flexbox grid system for [inuitcss framework](http://www.inuitcss.com).

## Work in progress

This is a work in progress. Use it at your own risk !  
Checkout the [develop branche](https://github.com/alienlebarge/inuit-flexbox/tree/develop) and the [pull requests](https://github.com/alienlebarge/inuit-flexbox/pulls) if you want to know what are the next features.

## Manual

### Gride type

#### Flexible grid

Flexible grid use columns wich are not fixed. They will fill the space available.
For exemple a column with a flex ratio of 2 will be twice larger than a clumn with
a flex ratio of 1.
If flexible grid is what you need, use the class `flex--flex`.

    <div class="flex flex--flex">
      <div class="flex__item--1"><div class="box"><code>.flex__item--1</code></div></div>
      <div class="flex__item--2"><div class="box"><code>.flex__item--2</code></div></div>
      <div class="flex__item--1"><div class="box"><code>.flex__item--1</code></div></div>
    </div>

#### Fixed grid

Fixed grid is based on a 12 columns system.
Use the `flex--fix` if you want a fixed grid.

    <div class="flex flex--fix">
      <div class="flex__item--1"><div class="box"></div></div>
      <div class="flex__item--11"><div class="box"></div></div>
    </div>
