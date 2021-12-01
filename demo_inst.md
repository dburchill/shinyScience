# demo steps

   ## initial layout

   1. move nav to after main, for screen readers

   2. add `display: flex` to container making it the flex container

      1. show child elements flow in row, fill to available space

   3. add `flex-wrap: wrap` to make elements wrap for responsive behaviour

      1. show wrapping behaviour

   4. set flex on elements   `flex: grow shrink basis` 

      1.  **header** span row `flex: 1 0 100%`  grow 1, don't shrink, fill row
      2.  **footer** same thing `flex: 1 0 100%`

   5. change order, **show** header, nav, sidebar, main, footer, `order: 1`

   6. change relative size of elements using flex property 

   7. nav and aside same size `flex 1 0 200px;` for nav & aside `flex 1 1 500px` for main 

   Nav, main, aside, 

   * set all to same grow so they expand together
   * nav and aside shrink 0 so they wont shrink smaller than their basis
   * main shrink to 1 so it will shirnk smaller than it's basis
   * set bassis 200px for nav & aside, 500px for main. 

   **note** 

   * on using absolute size (px) this is to set basis for flex, these are still alowed to grow and shrink acording to flex rules. 
   * responsive without media queries, flows in a row, we control order, basis size, how it grows and shrinks. 

   ## max size and center

   could set max width and margin on container to center and set a max size

   ```
   max-width: 1000px;
   margin: 0 auto;
   ```

   the flexbox way, make the containing element a flex box, center justified. 

   ``` 
   display: flex;
   justify-content: center;
   ```

   It has one child element, the container, give it flex properties, don't alow grow 0, alow shrink, basis size 1000px `flex: 0 1 1000px;`

​      