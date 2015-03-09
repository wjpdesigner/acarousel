# A.Carousel
A simple Bootstrap carousel with touch screen swipe ability.

[Checkout the demo](http://wjpdesigner.com/acarousel/)

[![Image of ACarousel](http://wjpdesigner.com/acarousel/screenshot.png?1)](http://wjpdesigner.com/acarousel/)

### Feature:
- Fully Responsive
- Swipe Ability
- Minimalist Design
- Easy to use just 3 steps

### Implementation:
#### 1.Getting Started
Load jQuery, Bootstrap and ACarousel files.
```html
<!--CDNs-->
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.2/css/bootstrap.min.css">
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/font-awesome/4.3.0/css/font-awesome.min.css">
<script src='https://code.jquery.com/jquery-1.11.2.min.js'></script>
<script src="https://code.jquery.com/ui/1.11.3/jquery-ui.min.js"></script>
<script src="https://code.jquery.com/mobile/1.4.5/jquery.mobile-1.4.5.min.js"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.2/js/bootstrap.min.js"></script>

<!--ACarousel include-->
<link rel="stylesheet" href="acarousel.css">
<script src="acarousel.js"></script>
```
#### 2.Set up your HTML
Make sure to keep the `id` (for example "#myCarousel") corresponding with the indicator (dots) and the controller (arrows).
It is not necessary to include dots and arrows, but the very first ".item" the ".active" `class` needs to be added to activate the slider.
```html
<!--START myCarousel-->
<div id="myCarousel" class="carousel slide" data-ride="carousel" data-interval="false" data-wrap="true" data-pause="hover">
		
	<!-- Dots -->
  	<ol class="carousel-indicators">
    	<li data-target="#myCarousel" data-slide-to="0" class="active"></li>
    	<li data-target="#myCarousel" data-slide-to="1"></li>
    	<li data-target="#myCarousel" data-slide-to="2"></li>
    	<li data-target="#myCarousel" data-slide-to="3"></li>
  	</ol>
  		
  	<!--Slides-->
  	<div class="carousel-inner">
  		<div class="item active">
  			<img src="img/slide1.jpg">
  			<!--Add your caption here-->
  			<!--div class="carousel-caption">
    			<h3>Title</h3>
    			<p>Description</p>
  			</div-->
		</div>
		<div class="item">
  			<img src="img/slide2.jpg">
		</div>
		<div class="item">
  			<img src="img/slide3.jpg">
		</div>
		<div class="item">
  			<img src="img/slide4.jpg">
  			<div class="carousel-caption">
    			<h3>Jane’s Carousel</h3>
    			<p>Built in 1922 by the Philadelphia Toboggan Company, the carousel was lovingly restored and donated to the park by Jane and David Walentas. Located in the Empire Fulton Ferry section of Brooklyn Bridge Park, Jane’s Carousel is housed in a gorgeous glass pavilion, designed by Pritzker-prize winning architect Jean Nouvel.</p>
  			</div>
		</div>
	</div>
		
	<!-- Arrows -->
  	<a class="left carousel-control" href="#myCarousel" role="button" data-slide="prev">
  		<i class="fa fa-angle-left" style="left:50%;"></i>
  	</a>
  	<a class="right carousel-control" href="#myCarousel" role="button" data-slide="next">
    	<i class="fa fa-angle-right"style="right:50%;"></i>
  	</a>
  		
</div><!--END myCarousel-->
```
#### 3.Config your carousel via data attributes
In the very first line options can be passed via data attributes.
<table class="table" width="100%">
	<thead>
		 <tr>
    		<th width="20%">Name</th>
    		<th width="15%">Type</th>
    		<th width="15%">Default</th>
    		<th width="50%">Description</th>
  		</tr>
  	</thead>
  	<tbody>
  		<tr>
    		<td>data-ride</td>
    		<td>string</td>
    		<td>"carousel"</td>
    		<td>The attribute is used to mark a carousel as animating starting at page load.</td>
  		</tr>
  		<tr>
    		<td>data-interval</td>
    		<td>number</td>
    		<td>5000</td>
    		<td>The amount of time to delay between automatically cycling an item. If false, carousel will not automatically cycle.</td>
  		</tr>
  		<tr>
    		<td>data-wrap</td>
    		<td>boolean</td>
    		<td>true</td>
    		<td>Whether the carousel should cycle continuously or have hard stops.</td>
  		</tr>
  		<tr>
    		<td>data-pause</td>
    		<td>string</td>
    		<td>"hover"</td>
    		<td>Pauses the cycling of the carousel on mouseenter and resumes the cycling of the carousel on mouseleave.</td>
  		</tr>
	</tbody>
<table>

### Copyright and License:
The MIT License (MIT)

Copyright (c) 2015 wjpdesigner.com

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.