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

