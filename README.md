# Interview Questions

### General Questions

* What did you learn yesterday/this week?

	* I learned some basic computer science concepts this week, such as Big-O notation, linked lists, and binary search.

* What excites or interests you about coding?

	* I really enjoy the challenge of it, and the gratification of creating something from nothing. It feels like I'm doing intricate puzzles every day, and it's very satisfying when it all comes together.



### HTML Questions

* What does a doctype do?

	* A doctype simply tells the browser what kind of markup language the page is written in.

* What's the difference between HTML and XHTML?

	* XHTML is very similar to HTML, but with a few differences. In XHTML, the doctype declaration is mandatory, as are the `<head>`, `<title>`, and `<body>` tags.  Additionally, even self-closing tags, like `<br>`, require a slash - `<br/>`.

* What are data- attributes good for?

	* The data attribute is meant to store additional data in an element that may not be displayed on the page. It can then be manipulated in its' JS page.

* Describe the difference between a cookie, sessionStorage and localStorage.

	* sessionStorage is only available while the browswer window is open.
	* localStorage can store large amounts of data
	* cookies only store strings, but are generally more secure than either local- or sessionStorage. also used for authentication

* Why is it generally a good idea to position CSS `<link>`s between `<head></head>` and JS `<script>`s just before `</body>`? Do you know any exceptions?

	* Placing the CSS `<link>` in the `<head>` section loads the styling before the page starts to render, so users see things like background colors as the page loads.

### CSS Questions

* What is the difference between classes and IDs in CSS?
	* IDs can only be used once, while classes can be used many times. IDs have a higher specificity, so an ID's properties will take precedence.

* What's the difference between "resetting" and "normalizing" CSS? Which would you choose, and why?

	* Reset gets rid of all browser styling, which means all styling must be done manually. Normalize tries to take care of any cross-browser differences and make them as consistent as possible.

* Describe Floats and how they work.
	* A float pushes an element to either the left or right, and if it's, say, a picture, text will flow around the picture to fill space.

* Describe z-index and how stacking context is formed.
	* Z-index is what determines vertical stacking order, or overlap. the higher the number, the more likely it is that that element will be stacked on top (or most visible).

* Have you ever used a grid system, and if so, what do you prefer?
	* Yes. I've used Materialize and Bootstrap. I prefer Materialize's documentation, but Bootstrap seems to be easier to customize/overwrite.

* Have you used or implemented media queries or mobile specific layouts/CSS?
	* Yes, both by using frameworks like Boostrap and by defining my own media queries.

* How do you optimize your webpages for print?
	* By having a separate css file that only gets applied when printing.

* What are the advantages/disadvantages of using CSS preprocessors?
	* A big advantage is organization, as well as more structured code. A disadvantage is that the nesting of selectors can get long very quickly.

* Explain how a browser determines what elements match a CSS selector.
	* As the browser parses the HTML, it reads the selectors from right to left and applies CSS when a match is found. If nothing is found, the rule is not used.

* Explain your understanding of the box model and how you would tell the browser in CSS to render your layout in different box models.
	* the 3 (or 4) components to the box model are the element itself, its padding, its border, and its margin. Increasing padding increases the space from the edge of the element and the content within the element, making it appear stretched. Border refers to the space between the padding and before the element's edge. Margin is the space directly on the outside of the element.


* What does * { box-sizing: border-box; } do? What are its advantages?
	* This sets the box model to the well-known border-box. This is for older browsers that may not support the border-box by default.

* What's the difference between inline and inline-block?
	* Displaying an element as inline-block allows you to give the element a height and still display it like an inline element.

* What's the difference between a relative, fixed, absolute and statically positioned element?
	* 

### JS Questions

### Database Questions

### Ruby/Rails

### Testing Questions

### Coding Questions

* Question: What is the value of foo? 
	* 1020 prints out as an integer, which means JavaScript is smart enough to parse the '20' into 10 as an integer of 1020.
```Javascript 
var foo = 10 + '20';
```

* Question: How would you make this work?

```Javascript
add(2, 5); // 7
add(2)(5); // 7

	function add(a, b) {
	return a + b;
	}

	function add(a) {
		return function(b) {
			return a + b;
		}
	}
```

* Question: What value is returned from the following statement?
	* goh angasal a m'i

```JavaScript
"i'm a lasagna hog".split("").reverse().join("");
```

* Question: What is the outcome of the two alerts below?
	* The result is a popup that says 'Hello World,' as well as an undefined message in the console that says 'bar' is not defined. Bar is not defined because it's only defined within the scope of the function call and does not exist outside of the function. Calling 'bar' in the alert is calling a variable that is not defined.

```Javascript
var foo = "Hello";
(function() {
  var bar = " World";
  alert(foo + bar);
})();
alert(foo + bar);
```
* Question: What is the value of foo.length?
 * 2

 ```Javascript
var foo = [];
foo.push(1);
foo.push(2);
 ```

* Question: What is the value of foo.x?

	* undefined

```Javascript
var foo = {n: 1};
var bar = foo;
foo.x = foo = {n: 2};
```

* Question: What does the following code print?

	* one
	  three
	  two

	```Javascript
	console.log('one');
	setTimeout(function() {
  		console.log('two');
		}, 0);
	console.log('three');
	```