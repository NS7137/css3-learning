# Flexbox

- for building 1-dimensional layouts
- automatically divided by its child elements
- align items to one anther inside a parent container, both horizontally and vertically
- sovles problems as vertical centering and equal-height columns
- replacing floats

## Flexbox Terminology

- Flex container
  - display: flex;
  - gap: 0 | length
    - space between items, without using margin
  - justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly
    - align items along main axis (horizontally, by default)
  - align-items: strtch | flex-start | flex-end | center | baseline
    - align items along cross axis (vertically, by default)
  - flex-direction: row | row-reverse | column | column-reverse
    - define which is the main axis
  - flex-wrap: nowrap | wrap | wrap-reverse
    - allow items to wrap into a new line if they are too large
  - align-content: strtch | flex-start | flex-end | center | space-between | space-around
    - only applies when there are multiple lines (flex-wrap: wrap)
- Flex items
  - align-self: auto | stretch | flex-start | flex-end | center | baseline
    - overwrite align-items for individual flex items
  - flex-grow: 0 | integer
    - allow an element to grow (0 means no, 1+ means yes)
    - 按比例增长
  - flex-shrink: 1 | integer
    - allow an element to shink (0 means no, 1+ means yes)
  - flex-basis: auto | length
    - define an item's width, instead of the width property
  - flex: 0 1 auto | int int len
    - recommended shorthand for flex-grod, -shrink, -basis.
  - order: 0 | integer
    - controls order of items. -1 makes item first, 1 makes it last
- main axis and cross axis 可以改变轴方向
  - 必须知道正在处理的是哪个轴

# CSS Grid

- building 2-dimensional layouts
- divide a container element into rows and columns
- less nested HTML and easier-to-read CSS
- not meant to replace flexbox. Need a 1D layout? Use flexbox. Need a 2D layout? Use CSS Grid.

## GRID CONTAINER

- grid-template-rows: track size
- grid-template-columns: track size
  - one length unit for each track.
- gap: 0 | length
- row-gap: 0 | length
- column-gap: 0 | length
  - create empty space between tracks
- justify-items: stretch | start | center | end
- align-items: stretch | start | center | end
  - align items inside rows/columns
- justify-content: start | center | end
- align-content: start | center | end
  - align entire grid inside grid container.Only applies if container is larger than the grid

## GRID ITEMS

- grid-column: start line / end line | span number
- grid-row: start line / end line | span number
  - place a grid item into a specific cell, based on line numbers.
  - span keyword can be used to span an item across more cells
- justify-self: stretch | start | center | end
- align-self: stretch | start | center | end
  - to overwrite justify-items / align-items for single items

# Select Breakpoint

- Bad based on popular devices
- Good based on screen width ranges
  - 1200px(900-1100) 900px(600-900) 600px(300-600)
- Perfect when design breaks down

# JS part

- Set current year
- Make mobile navigation work
- Smooth scrolling animation
- Sticky navigation
