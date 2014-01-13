# [BLESS LESS Mixins](https://github.com/BlowbackDesign/BLESS)

## CSS Properties

### `.background-clip(@clip)`

http://www.w3.org/TR/css3-background/#the-background-clip

```
.background-clip(content-box);
```

### `.background-size(@size)`

http://www.w3.org/TR/css3-background/#the-background-size

```
.background-size(128px 32px);
```

### `.border-radius(@radius)`

 * `.border-top-left-radius(@radius)`
 * `.border-top-right-radius(@radius)`
 * `.border-bottom-right-radius(@radius)`
 * `.border-bottom-left-radius(@radius)`

http://www.w3.org/TR/css3-background/#the-border-radius

```
.border-radius(32px 0 0 32px);
```

### `.box-shadow(@shadow)`

 * `.box-shadow("@shadow[, @shadow]...")`

http://www.w3.org/TR/css3-background/#box-shadow

```
.box-shadow(1px 1px 6px #333);
```

### `.box-sizing(@size)`

http://www.w3.org/TR/2002/WD-css3-box-20021024/#box-sizing

```
.box-sizing(border-box);
```

### `.column-count(@count)`

http://www.w3.org/TR/css3-multicol/#column-count

```
.column-count(6);
```

### `.column-gap(@gap)`

http://www.w3.org/TR/css3-multicol/#column-gap

```
.column-gap(32px);
```

### `.opacity(@opacity[, @ie])`

 * `.ie-opacity(@opacity)`

http://www.w3.org/TR/2003/CR-css3-color-20030514/#transparency

```
.opacity(0.5, true);
```

### `.transform(@function)`

http://www.w3.org/TR/css3-transforms/#transform-property

```
.transform(rotate(70deg) translate(64px));
```

### `.transform-origin(@origin)`

http://www.w3.org/TR/css3-transforms/#transform-origin-property

```
.transform-origin(left bottom);
```

### `.transform-style(@style)`

http://www.w3.org/TR/css3-transforms/#transform-style-property

```
.transform-style(preserve-3d);
```

### `.transition(@transition)`

 * `.transition("@transition[, @transition]...")`

http://www.w3.org/TR/css3-transitions/#transition-shorthand-property

```
.transition(all 2s);
```

### `.transition-delay(@transition-delay)`

http://www.w3.org/TR/css3-transitions/#transition-delay-property

```
.transition-delay(0.5s);
```

### `.transition-duration(@transition-duration)`

http://www.w3.org/TR/css3-transitions/#transition-duration-property

```
.transition-duration(0.5s);
```

### `.transition-property(@transition-property)`

http://www.w3.org/TR/css3-transitions/#transition-property-property

```
.transition-property(width height);
```

### `.transition-timing-function(@transition-timing-function)`

http://www.w3.org/TR/css3-transitions/#transition-timing-function

```
.transition-timing-function(ease-out);
```

### `.user-select(@select)`

http://www.w3.org/TR/2000/WD-css3-userint-20000216#user-select

```
.user-select(none);
```

## Transform Functions

### `.rotate(@degrees)`

Shortcut to **rotate transform function**.

http://www.w3.org/TR/css3-transforms/#rotate-function

```
.rotate(35);
```

### `.scale(@ratio)`

Shortcut to **scale transform function**.

http://www.w3.org/TR/css3-transforms/#scale-function

```
.scale(1.5);
```

### `.skew(@x[, @y])`

Shortcut to **skew transform function**.

http://www.w3.org/TR/css3-transforms/#skew-function

```
.skew(35);
```

### `.translate(@x[, @y])`

Shortcut to **translate transform function**.

http://www.w3.org/TR/css3-transforms/#translate-function

```
.translate(-128px, -32px);
```

### `.translate3d(@x, @y, @z)`

Shortcut to **translate3d transform function**.

http://www.w3.org/TR/css3-transforms/#translate3d-function

```
.translate3d(-128px, -32px,  32px);
```

## CSS Helpers

### `.columns(@count[, @gap])`

Content columns shortcut to **column-count** with **column-gap**.

```
.columns(4, 20px);
```

### `.font-size(@font-size)`

Set px/rem font-size.

```
.font-size(24);
```

### `.rounded(@radius)`

 * `.rounded-top-left(@radius)`
 * `.rounded-top-right(@radius)`
 * `.rounded-bottom-right(@radius)`
 * `.rounded-bottom-left(@radius)`

Shortcut to **border-radius**.

```
.rounded(64px);
```

### `.size(@width[, @height])`

 * `.min-size(@width[, @height])`
 * `.max-size(@width[, @height])`

Sizing mixins to set element width / height. One argument adds value to both properties.

```
.size(256px, 128px);
```

### `.spacing(@margin[, @padding])`

Spacing mixin to set element margin / padding. One argument adds value to both properties.

```
.spacing(10px);
```

## PSD Layer Style

### `.drop-shadow([@x[, @y[, @blur[, @spread[, @color[, @alpha]]]]]])`

 * `.drop-shadow(@x @y @blur @spread @color @alpha)`
 * `.drop-shadow(@x @y @blur @spread @color)`
 * `.drop-shadow(@x @y @blur @color @alpha)`
 * `.drop-shadow(@x @y @blur @color)`

Shortcut to **box-shadow**.

```
.drop-shadow(1px 1px 6px #000 0.6);
```

### `.inner-shadow([@x[, @y[, @blur[, @spread[, @color[, @alpha]]]]]])`

 * `.inner-shadow(@x @y @blur @spread @color @alpha)`
 * `.inner-shadow(@x @y @blur @spread @color)`
 * `.inner-shadow(@x @y @blur @color @alpha)`
 * `.inner-shadow(@x @y @blur @color)`

Shortcut to **inset box-shadow**.

```
.inner-shadow(0 3px 9px #fff 0.9);
```

### `.stroke([@color[, @alpha[, @size]]])`

 * `.stroke(@color, @alpha, @size, @string)`
 * `.stroke(@color, @alpha, @string)`
 * `.stroke(@color, @string)`

Crappy stroke created by four text shadows. `@string` can take optional extra text shadow(s) as string.

## CSS Colors

### `.background-color(@color[, @alpha])`

Background color with alpha opacity.

```
.background-color(purple, 0.6);
```

### `.border-color(@color[, @alpha])`

Border color with alpha opacity.

```
.border-color(red green blue, 0.6);
```

### `.color(@color[, @alpha])`

Color with alpha opacity.

```
.color(blue, 0.8);
```

### `.linear-gradient(@angle, @color[, @position[, @alpha]])`

 * `.linear-gradient-top(@color[, @position[, @alpha[, @ie]]])`
 * `.linear-gradient-top-right(@color[, @position[, @alpha]])`
 * `.linear-gradient-right(@color[, @position[, @alpha[, @ie]]])`
 * `.linear-gradient-bottom-right(@color[, @position[, @alpha]])`
 * `.linear-gradient-bottom(@color[, @position[, @alpha[, @ie]]])`
 * `.linear-gradient-bottom-left(@color[, @position[, @alpha]])`
 * `.linear-gradient-left(@color[, @position[, @alpha[, @ie]]])`
 * `.linear-gradient-top-left(@color[, @position[, @alpha]])`
 * `.ie-linear-gradient-top(@color[, @alpha])`
 * `.ie-linear-gradient-right(@color[, @alpha])`
 * `.ie-linear-gradient-bottom(@color[, @alpha])`
 * `.ie-linear-gradient-left(@color[, @alpha])`

Linear gradient with *unlimited* color / position breakpoints and alpha opacity support.

```
.linear-gradient-left(red orange yellow green blue, 0% 25% 50% 75% 100%);
```