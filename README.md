# CSS Position Demo

This is an html page that represents four types of positioning: static, relative, absolute, and fixed.

Static is the default. All positioning CSS rules are commented out. 
You can uncomment them to see their effect.

### Link

https://replit.com/@rmccrear/Class-04-CSS-Position

## Position values

### Static

`position: static` is the default. It will ignore all positioning CSS rules like `left`, `right`, `top`, and `bottom`. It will also ignore `z-index`.

### Relative

`position: relative` will allow you to move the item left, right, up or down, "relative to itself". 

It will move up with `top: -10px` or down with `top: 10px`.

`left`, `right`, `top`, and `bottom` will move the element relative to its own place in the document flow.

It can have a `z-index` set to positive or negative values. It can also serve as a container for containers with absolute positioning.

Moving the element will leave a blank place in the document where it would have been with moving it.

### Absolute

If you set an ancestor element to `relative`, `position: absolute` can be used to move an item around within a containing block. So, for example, `bottom: 10px` would place it 10px above the bottom of that ancestor element.

If there is not ancestor element that is positioned with `relative` (or any value like `absolute`, `fixed`, etc...), it will be placed relative to the `initial containing block`, which is something like the initial viewport.

### Fixed

This will place the element relative to the `intitial containing block`, which is something like the initial viewport. (But it will still be effected by CSS Transforms, if you use them.)