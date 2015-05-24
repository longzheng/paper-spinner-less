# paper-spinner-less
LESS version of [Google's Paper Spinner element](https://github.com/polymerelements/paper-spinner)

## Demo
https://cdn.rawgit.com/longzheng/paper-spinner-less/master/demo.html
![spinner](https://cloud.githubusercontent.com/assets/484912/7788146/60329bb2-0272-11e5-9430-5f680fc43fa0.gif)

## How to use
Include the CSS
```html
<link rel="stylesheet" href="paper-spinner.css" />
```
Insert the spinner template. Unfortunately due to the way the spinner is animated, the HTML template is quite big heavily nested. Might be useful to use a frontend framework like Angular to turn this into a template include.
```html
<div class="paper-spinner">
	<div class="spinner-container active">
		<div class="spinner-layer layer-1">
			<div class="circle-clipper left">
				<div class="circle"></div>
			</div><div class="gap-patch">
				<div class="circle"></div>
			</div><div class="circle-clipper right">
				<div class="circle"></div>
			</div>
		</div>
		<div class="spinner-layer layer-2">
			<div class="circle-clipper left">
				<div class="circle"></div>
			</div><div class="gap-patch">
				<div class="circle"></div>
			</div><div class="circle-clipper right">
				<div class="circle"></div>
			</div>
		</div>
		<div class="spinner-layer layer-3">
			<div class="circle-clipper left">
				<div class="circle"></div>
			</div><div class="gap-patch">
				<div class="circle"></div>
			</div><div class="circle-clipper right">
				<div class="circle"></div>
			</div>
		</div>
		<div class="spinner-layer layer-4">
			<div class="circle-clipper left">
				<div class="circle"></div>
			</div><div class="gap-patch">
				<div class="circle"></div>
			</div><div class="circle-clipper right">
				<div class="circle"></div>
			</div>
		</div>
	</div>
</div>
```

## Customize
In the LESS file, you can customize the color options by using the mixin.
```less
// Custom color
.paper-spinner.custom {
	.paper-spinner(#00fc38);
}
```
Then add the class in your HTML
```html
<div class="paper-spinner red">
```
