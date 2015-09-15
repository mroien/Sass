#Sass

## Tutorial from [thenewboston](https://www.youtube.com/playlist?list=PL6gx4Cwl9DGBxQO2r_kmxn-0UqL_Rkj0t)

### Creating Variables
```CSS
$button-color: white;

.button {
	color: $button-color;
}
```

### Mixins
```CSS
@mixin border-radius ($radius) {
	-webkit-border-radius: $radius;
	-moz-border-radius: $radius;
	-ms-border-radius: $radius;
	border-radius: $radius;
}
.panel {
	@include border-radius(5px);
	}
```

### Extends
- Use @extend .button in the object you want to extend it to
```CSS
.button2.0 {
	@extend .button;
	ADD MORE STUFF
}
```

### Operations
- multiple a variable greater than 1 to make it lighter
- multiple a varialbe less than 1 to make it darker
- you can add + 30 you don't need the px or em Sass know what to add

### Import
- You name the new file _filename.scss
- on page you want to import it into, top of page @import "filename" 
- You leave off the underscore and file extension
