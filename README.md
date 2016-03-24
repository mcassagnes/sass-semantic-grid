# css-semantic-grid
Simple css grid system to help you keep your HTML markup semantic-oriented.

#####This is not easy to read
```html
<div class="grid">
  <div class="col-1-3">
    <div class="item">
      <!-- more markup -->
    </div>
  </div>
</div>
```

#####This makes more sense
```html
<div class="items">
  <div class="item>
    <!-- more markup -->
  </div>
</div>
```

##Usage
```css
.items {
  @extend %block-container;
  
  .item {
    @extend %grid-block;
    @include grid(1/3);
  }
}
```
