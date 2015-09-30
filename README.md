## Website Performance Optimization portfolio project


### Outline

#### Part 1: Index Pages

1. All external image links are saved under img directory.
2. Optimize images to a smaller size
3. Inline css
4. Move Javascript to the end of the page for faster load speed
5. Added will-change to .move class


#### Part 2: Pizza

views/js/main.js

1. LINE: 522 -- updatePositions()
  
  Set array of phases to reduce layout calls, limit the cause of asynchrnous layout
  Added requestionAnimationFrame when calling updatePosition to boost speed

2. LINE: 563 -- DOMContentLoaded
  Added windowHeight variable which checks the height of the window and determins the number of pizza to render on page.

3. LINE 487 -- pizzasDIV
  Move pizzaDiv outside of the loop.

4. LINE 453 -- changePizzaSizes()
  Remove determinDX as it is not needed. Added switch statment to changePizzaSize as the size is given from changeSliderLabel. changePizzaSize can apply the new style to the element.
