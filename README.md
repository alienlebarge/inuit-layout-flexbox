# inuit-flexbox

A flexbox grid system for [inuitcss framework](http://www.inuitcss.com).

## Work in progress

This is a **work in progress**. Use it at your own risk !

If you want to help, you are welcome.  
If you see features that made sense to be added, feel free to [open an issue](https://github.com/alienlebarge/inuit-flexbox/issues/new).

## Manual

### Gride type

There two type of grid system: on that's use flexbox `flex-grow` propertie and one that is more traditional who use a 12 columns width grid system.

#### Flexible grid

Flexible grid use flexbox `flex-grow` propertie. To enable it, set `$inuit-flexbox-flex-grid-enable: true`.

    <div class="layout layout--flex">
        <div class="layout__item
                    layout__item--1">
        </div>
        <div class="layout__item
                    layout__item--2">
        </div>
        <div class="layout__item
                    layout__item--1">
        </div>
    </div>

#### Fixed grid

This grid system is based on a 12 columns width architecture. You can enable it by setting `$inuit-flexbox-fixed-grid-enable: true`.  
You can also change the number of columns with the variable `$inuit-flexbox-columns-number`.

    <div class="layout layout--fixed">
        <div class="layout__item
                    layout__item--1">
        </div>
        <div class="layout__item
                    layout__item--2">
        </div>
        <div class="layout__item
                    layout__item--1">
        </div>
    </div>

### Width depending on viewport

    <div class="layout--flex">
        <div class="layout__item
                    layout__item--full
                    layout__item--lap-and-up--1
                    layout__item--desk--1">
        </div>
        <div class="layout__item
                    layout__item--1
                    layout__item--lap-and-up--2
                    layout__item--desk--4">
        </div>
        <div class="layout__item
                    layout__item--1
                    layout__item--lap-and-up--1
                    layout__item--desk--2">
        </div>
    </div>

### Order

    <div class="layout layout--flex">
        <div class="layout__item
                    layout__item--1
                    layout__item--order-2">
        </div>
        <div class="layout__item
                    layout__item--1
                    layout__item--order-3">
        </div>
        <div class="layout__item
                    layout__item--1
                    layout__item--order-1">
        </div>
    </div>

#### Order depending on viewport

    <div class="layout layout--flex">
        <div class="layout__item
                    layout__item--full
                    layout__item--lap-and-up--order-2
                    layout__item--desk--order-3">
        </div>
        <div class="layout__item
                    layout__item--1
                    layout__item--lap-and-up--order-1
                    layout__item--desk--order-2">
        </div>
        <div class="layout__item
                    layout__item--1
                    layout__item--lap-and-up--order-3
                    layout__item--desk--order-1">
        </div>
    </div>

### Reverse

    <div class="layout layout--flex layout--reverse">
        ...
    </div>

### Offset

Offsets are only available for `.layout--fixed` grid.

    <div class="layout layout--fixed">
      <div class="layout__item
                  layout__item--6
                  layout__item--offset-6">
      </div>
    </div>

#### Responsive offset

    <div class="layout layout--fixed">
      <div class="layout__item layout__item--1
                  layout__item--palm--offset-2
                  layout__item--lap--offset-5
                  layout__item--desk--offset-11">
      </div>
    </div>
