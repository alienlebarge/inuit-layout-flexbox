# inuit-flexbox

A flexbox grid system for [inuitcss framework](http://www.inuitcss.com).

## Work in progress

This is a **work in progress**. Use it at your own risk !

If you want to help, you are welcome.

## Manual

### Gride type

There two type of grid system: on that's use flexbox `flex-grow` propertie and one that is more traditional who use a 12 columns width grid system.

#### Flexible grid

Flexible grid use flexbox `flex-grow` propertie.
To enable it, set `$inuit-flexbox-flex-grid-enable: true`.

    <div class="flex flex--flex">
        <div class="flex__item
                    flex__item--1">
        </div>
        <div class="flex__item
                    flex__item--2">
        </div>
        <div class="flex__item
                    flex__item--1">
        </div>
    </div>

#### Fixed grid

This grid system is based on a 12 columns width architecture.
You can enable it by setting `$inuit-flexbox-fixed-grid-enable: true`.
You can also change the number of columns with the variable `$inuit-flexbox-columns-number`

    <div class="flex flex--fixed">
        <div class="flex__item
                    flex__item--1">
        </div>
        <div class="flex__item
                    flex__item--2">
        </div>
        <div class="flex__item
                    flex__item--1">
        </div>
    </div>

### Width depending on viewport

    <div class="flex--flex">
        <div class="flex__item
                    flex__item--full
                    flex__item--lap-and-up--1
                    flex__item--desk--1">
        </div>
        <div class="flex__item
                    flex__item--1
                    flex__item--lap-and-up--2
                    flex__item--desk--4">
        </div>
        <div class="flex__item
                    flex__item--1
                    flex__item--lap-and-up--1
                    flex__item--desk--2">
        </div>
    </div>

### Order

    <div class="flex flex--flex">
        <div class="flex__item
                    flex__item--1
                    flex__item--order-2">
        </div>
        <div class="flex__item
                    flex__item--1
                    flex__item--order-3">
        </div>
        <div class="flex__item
                    flex__item--1
                    flex__item--order-1">
        </div>
    </div>

#### Order depending on viewport

    <div class="flex flex--flex">
        <div class="flex__item
                    flex__item--full
                    flex__item--lap-and-up--order-2
                    flex__item--desk--order-3">
        </div>
        <div class="flex__item
                    flex__item--1
                    flex__item--lap-and-up--order-1
                    flex__item--desk--order-2">
        </div>
        <div class="flex__item
                    flex__item--1
                    flex__item--lap-and-up--order-3
                    flex__item--desk--order-1">
        </div>
    </div>

### Reverse

    <div class="flex flex--flex flex--reverse">
        ...
    </div>
