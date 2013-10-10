columnus
========

Stylus responsive grid system based loosely off of the Foundation 12-column grid.

##Usage

Columnus uses predefined html classes setup in the stylus file. Each number is based off of a twelve column grid system, similar to that of Foundation. Read more [here](http://foundation.zurb.com/docs/components/grid.html).

In the example below, you'll get two columns at your smallest breakpoint, three at your medium one, and 4 at your largest:

```html
<div class="l_grid">
  <div class="small_6 med_4 large_3 l_column">...</div>
  <div class="small_6 med_4 large_3 l_column">...</div>
  <div class="small_6 med_4 large_3 l_column">...</div>
  <div class="small_6 med_4 large_3 l_column">...</div>
</div>
```

Note: This uses the layout class naming, taken from [SMACSS](http://smacss.com/).

Special thanks to the Foundation crew. Their code rocks, and was the inspiration for this simple grid system.
