# Practicing Responsive Grids

## Working Together

Using the example above, let's complete the following:

1. Use a `grid` to put the `.logo` and `.nav-btn` into the same row. Align the logo to the left the button to the right.
    - This can be done using `text align` (left/right), or `justify-self` (start/end).
2. Set the `.nav-menu` to span across two columns using `grid-column`

```
   ---------------------------
   |   .logo   |  .nav-btn   |
   ---------------------------
   |        .nav-menu        |
   ---------------------------
```

3. Create a `@media` query at `min-width: 640px` (or equivalent) and turn the `.lessons-grid` into a `grid` with a template of two columns.
4. Apply a `grid-gap` of 1em (or equivalent) to the `.lessons-grid`.
    - Be sure to remove the margin on each `.lesson` to get an evenly spaced layout.
    - Note you could also go back and setup the `.lessons-grid` as a single-column grid (or no specified template) with grid-gap from the onset, to prevent having to override the margin. A grid-gap, in this example, can achieve the same spacing as the margin.
5. Create a `@media` query at `min-width: 900px` (or equivalent) and turn the menu into something more suitable for a larger viewport, by:
    - Setting the `.nav-btn` to `display: none;` to remove it
    - Ensuring the `.header-block` only spans a single column
    - Setting all `.menu-item` elements to `display: inline-block;` (or, turn the `.mainmenu` into a `grid`!)

## On Your Own

Add any rules that do not already exist to complete the following:

1. Change the layouts of the `.lessons-grid` to be a 4 column grid within the `min-width:900px` breakpoint
      ```
      grid-template-columns: 1fr 1fr 1fr 1fr;
      ```

2. Restrict the maximum width of the `.main-block`, then ensure that block is centered within the layout
      ```
      max-width: 1200px;
      margin: 0 auto;
      ```

3. Continue the media query at 900px by turning `.main-block` into a grid that has the following template:
      ```
      ---------------------------
      |      .main-header       |
      ---------------------------
      |        .lessons         |
      ---------------------------
      |  .grading  |  .topics   |
      ---------------------------
      ```
      _Hint: Don't think about shrinking the last two elements into the single column, but instead think about stretching the first two across the template._
