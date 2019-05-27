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
