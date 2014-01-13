# BLESS

**Collection of usefull LESS mixins**

BLESS is compatible with [less.js](https://github.com/less/less.js) 1.4.2 or greater. It doesn't rely on any JavaScript evaluation so it's also compatible with most of less.js ports out there. Check out the full list of features and available mixins [from the docs](docs).

## Use

Include BLESS to your LESS stylesheet and we're ready to rumble:

```css
@import "../path/to/bless.less";
```
Throw in some BLESS mixins...

```css
.my-element {
	color: #222;
	.linear-gradient-top(#eee #fff #ccc, 0% 50% 100%);
	.rounded(6px);
	.spacing(0);
	.transition(all 0.3s);
	&:hover { .scale(1.5); }
}
```

...and enjoy the results:

```css
.my-element {
	color: #222;
	background: -webkit-gradient(linear, center top, center bottom, color-stop(0%, #eeeeee), color-stop(50%, #ffffff), color-stop(100%, #cccccc));
	background: -webkit-linear-gradient(-90deg, #eeeeee 0%, #ffffff 50%, #cccccc 100%);
	background: -moz-linear-gradient(-90deg, #eeeeee 0%, #ffffff 50%, #cccccc 100%);
	background: -ms-linear-gradient(-90deg, #eeeeee 0%, #ffffff 50%, #cccccc 100%);
	background: -o-linear-gradient(-90deg, #eeeeee 0%, #ffffff 50%, #cccccc 100%);
	background: linear-gradient(180deg, #eeeeee 0%, #ffffff 50%, #cccccc 100%);
	filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#ffeeeeee', endColorstr='#ffffffff', GradientType=0);
	-webkit-border-radius: 6px;
	-moz-border-radius: 6px;
	border-radius: 6px;
	margin: 0;
	padding: 0;
	-webkit-transition: all 0.3s;
	-moz-transition: all 0.3s;
	-o-transition: all 0.3s;
	transition: all 0.3s;
}
.my-element:hover {
	-webkit-transform: scale(1.5);
	-moz-transform: scale(1.5);
	-ms-transform: scale(1.5);
	-o-transform: scale(1.5);
	transform: scale(1.5);
}
```

## Licence

[The MIT License (MIT)](LICENCE.md)

Copyright (c) 2013 Blowback - https://github.com/BlowbackDesign