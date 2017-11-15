# Angled Edges (SASS mixin)

[Live demo](http://nigelotoole.github.io/angled-edges/)

Add a consistent angled edge to a full width element.
This technique uses only border for angled edges in a pseudo-element.
It is only intended for use on full width elements as it uses the vw unit to calulate the angle.


## Usage

Just import the partial and include it where needed.
```sass
@import 'path/to/angled-edges';

.here-i-need-an-angled-edge {
  @include angle-edge($angle, $angle-position-y, $angle-position-x, $color, $angle-position-bottom-x);
}
```
Where:
$angle: The angle in degrees: 1 - 45
$angle-position-y: The Y position of the angle: top | bottom | both
$angle-position-x: The X position of the angle: left | right
$color: Color of angled edge: Hex color
$angle-position-bottom-x: The X position of the bottom angle if using 'both' for $angle-position-y: left | right

### License
MIT © Nigel O Toole
