# LESS is MOAR

Aint your grandma's CSS helper. This is LESS, and it's MOAR.

## Getting started

* Clone the repo: `git clone git@github.com:ericmuyser/moar.git`
* Build away!

## Features

* Grid System - dynamic column/gutter grid system, and common structures
	* 12 Column/960px (960 Grid System)
	* Fluid/16px
	* 10 Column/1070px (Less Framework)
* Clearfix - standard clearfix ported to LESS.
* Reset - resets all elements.
* Helper - set of helper methods that abstract unnecessary details (commonly vendor prefixes).

## Structure

### all.less
Includes reset.less, clearfix.less, helper.less, and grid.less

### clearfix.less
* .clear-fix
* .clear-fix-after

### grid.less
* .column(@index, @column-width, @gutter-buffer, @float: left)
* .gutter(@index, @column-width, @float: left)

### grid-less.less
* .col-1 to .col-10
* .wrap-1 to .wrap-10

### grid-fluid-16.less
* .col-1 to .col-16
* .wrap-1 to .wrap-16

### grid-960-12.less
* .col-1 to .col-12
* .wrap-1 to .wrap-12

### helper.less
* .underline
* .hide-underline
* .hide-border-radius
* .hide-border
* .hide-shadow
* .hide-outline
* .hide-background
* .hide-text-shadow
* .hide-bullets
* .hide-overflow
* .disable-selection
* .hand
* .box-inside
* .italic
* .bold
* .strike
* .margin-center
* .text-left
* .text-right
* .text-center
* .relative
* .absolute
* .left
* .right
* .clear-both
* .clear-left
* .clear-right
* .block
* .inline
* .reset-dimensions
* .reset-width
* .hide
* .show
* .dimensions(@width, @height)
* .bw-gradient(@start: 0, @stop: 255) - black to white gradient
* .vertical-gradient(@color-1: #000, @color-2: #fff)
* .border(@top-color: #ccc, @right-color: #ccc, @bottom-color: #ccc, @left-color: #ccc)
* .drop-shadow(@x-axis: 0, @y-axis: 1px, @blur: 2px, @alpha: 0.1)
* .opacity(@opacity: 0.5)
* .transition-duration(@duration: 0.2s)
* .rotation(@deg: 5deg)
* .scale(@ratio: 1.5)
* .transition(@duration: 0.2s, @ease: ease-out)
* .inner-shadow(@color, @horizontal: 0, @vertical: 1px, @blur: 2px, @alpha: 1)
* .outer-shadow(@color, @horizontal: 0, @vertical: 1px, @blur: 2px, @alpha: 1)
* .text-shadow(@color, @horizontal: 0, @vertical: 1px, @blur: 2px)
* .columns(@width: 250px, @count: 0, @colgap: 50px, @rule-color: #EEE, @rule-style: solid, @rule-width: 1px)
* .box-inside
* .inner-outer-shadow(@inner-color, @inner-horizontal: 0, @inner-vertical: 1px, @inner-blur: 2px, @outer-color, @outer-horizontal: 0, @outer-vertical: 1px, @outer-blur: 2px)

### reset.less
None

## Usage

### Vertical Gradient
Add a vertical gradient from top to bottom:
```
a {
	.vertical-gradient(#ededed, #c4c4c4);
}
```

### Standard clearfix
Insert this code at the end of the parent element in which you would normally clearfix:
```
.clear-fix;
&:after { .clear-fix-after; }
```

### Border radius
Add a border radius to the left side of an anchor: 
```
a {
	.border-radius(5px, 5px, 10px, 10px);
}
```

### Inner/outer glow
Add an inner and outer shadow to an element:
```
a {
	.inner-outer-shadow(#bbb, 0, 0, 5px, #bbb, 0, 0, 5px);
}
```

### Text shadow
Add a text shadow to an element:
```
a {
	.text-shadow(#fff, 1px, 1px, 1px);
}
```

### Outer glow
Add an outer shadow to an element:
```
a {
	.outer-shadow(#000, 0px, 0px, 1px);
}
```

## Projects using moar

* [uTelevision.app](https://github.com/ericmuyser/jquery-ui-theme-cocoa)
* [jquery-ui-theme-cocoa](https://github.com/ericmuyser/jquery-ui-theme-cocoa)