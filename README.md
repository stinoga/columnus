columnus
========

Stylus responsive grid system based loosely off of the Foundation 12-column grid.

##Prerequisites
Install [Stylus](https://github.com/learnboost/stylus) and [Nib](https://github.com/visionmedia/nib).

##Usage

Add the columnus stylus file to your codebase, and import it into any stylus file you'd like to use the grid:

```sass
@import 'columnus'
```

##Breakpoints

The grid breakpoints are setup for a mobile-first design approach. You may change this to whatever style needed.

By default, the grid function will compile css classes with a prepend 'small'. You can change these class names by passing an agrument. In the below example, a grid is being setup at the base size below 48em. Then at the larger breakpoints, a medium and large grid are created.

```sass
grid()

@media '(min-width: 48em)'

  grid('med')

@media '(min-width: 64em)'

  grid('large')
```

##HTML

Columnus uses predefined html classes setup in the stylus file, as shown above. Each number is based off of a twelve column grid system, similar to that of Foundation. For example, a column spanning 6 of the 12 columns would be 50% of the parent element's width.

The example below uses the grid setup from above. you'll get two columns at your smallest breakpoint, three at your medium one, and 4 at your largest:

```html
<div class="l_grid">
  <div class="small_6 med_4 large_3 l_column">...</div>
  <div class="small_6 med_4 large_3 l_column">...</div>
  <div class="small_6 med_4 large_3 l_column">...</div>
  <div class="small_6 med_4 large_3 l_column">...</div>
</div>
```

Note: This uses the layout class naming scheme, taken from [SMACSS](http://smacss.com/).

Special thanks to the Foundation crew. Their code rocks, and was the inspiration for this simple grid system. Read more on the Foundation grid [here](http://foundation.zurb.com/docs/components/grid.html).
