# Bootstrap-basics
Learning bootstrap


```html
<div class="container">
    <h1>Our Print Sizes</h1>
    <div class="row">
        <div class="col-sm-6 col-md-3">Small</div>
        <div class="col-sm-6 col-md-3">Medium</div>
        <div class="col-sm-6 col-md-3">Large</div>
        <div class="col-sm-6 col-md-3">Extra Large</div>
    </div>
</div>
```

- We have retained col-md-3, but now we have included col-sm-6. This means that for viewports below 768 px in width, we want each element to take up six columns. This will result in the first two elements displaying on one line and the last two below that.

- On a viewport 768 px or wider, the categories appear in one horizontal row

``` html
<div class="container">
   <h1>Our Print Sizes</h1>
   <div class="row">
      <div class="col-6 col-sm-3">
         <h5>Small</h5>
         <div class="row">
            <div class="col-sm-4">6x5</div>
            <div class="col-sm-4">8x10</div>
            <div class="col-sm-4">11x17</div>
         </div>
      </div>
      <div class="col-6 col-sm-3">
         <h5>Medium</h5>
         <div class="row">
            <div class="col-sm-4">12x18</div>
            <div class="col-sm-4">16x20</div>
            <div class="col-sm-4">18x24</div>
         </div>
      </div>
      <div class="col-6 col-sm-3">
         <h5>Large</h5>
         <div class="row">
            <div class="col-sm-4">19x27</div>
            <div class="col-sm-4">20x30</div>
            <div class="col-sm-4">22x28</div>
         </div>
      </div>
      <div class="col-6 col-sm-3">
         <h5>Extra Large</h5>
         <div class="row">
            <div class="col-sm-4">24x36</div>
            <div class="col-sm-4">27x39</div>
            <div class="col-sm-4">27x40</div>
         </div>
      </div>
   </div>
</div>
```



```
<div class="col-sm-3">
      <h5>Extra Large</h5>
      <div class="row">
          <div class="col">24x36</div>
          <div class="col">27x39</div>
          <div class="w-100"></div>
          <div class="col">27x40</div>
      </div>
</div>
```

- The w-100 class simply sets the width of the element to 100%, forcing it to take up all the available horizontal space. Bootstrap offers a range of classes at a 25% interval: w-25, w-50, w-75, and w-100. Their vertical equivalents are h-25, h-50, h-75, and h-100.

```html
<div class="container">
    <h1>Our Print Sizes</h1>
    <div class="row justify-content-center">
      <div class="col-sm-6 col-md-3">Small</div>
      <div class="col-sm-6 col-md-3">Medium</div>
    </div>
    <div class="row justify-content-start">
      <div class="col-sm-6 col-md-3">Large</div>
      <div class="col-sm-6 col-md-3">Extra Large</div>
    </div>
    <div class="row justify-content-end">
      <div class="col-sm-6 col-md-3">Enormous</div>
      <div class="col-sm-6 col-md-3">Extra Enormous</div>
    </div>
</div>
```

- The alignment of each row can be customized, irrespective of the alignment of the previous or succeeding rows, that is, using the justify-content-start, justify-content-center, and justify-content-end classes, columns can be left-, right-, and center-aligned. For example, let's revert to our simple, unnested grid and arrange the grid in such a way that the columns on the first row are center-aligned and align the columns on the second and third row to the right and to the left, respectively. To do so, we simply add the justify-content-start class alongside the row to the first element, and the justify-content-start and justify-content-end classes to the following rows:
