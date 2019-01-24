# Technical skills test

This front end development test has been designed to assess a broad range of skills required to deliver high quality government digital services. This includes:

* Developing for accessibility
* HTML
* CSS
* JavaScript and associated frameworks/libraries
* Progressive enhancement and other best practices

## Instructions

Candidates are asked to perform this test remotely and **submit their responses to [gwyn.jones@nationalarchives.gov.uk](mailto:gwyn.jones@nationalarchives.gov.uk)**. Candidates are also welcome to email if anything needs clarification.

## Skills

### Accessibility

Describe how you would implement the front-end code (HTML, CSS and JavaScript) for tabbed search functionality similar to that appears which on The National Archives' [catalogue](http://discovery.nationalarchives.gov.uk/advanced-search). **This is not a design task and your answer should be focussed only on technical considerations**. You should assume all functionality and forms will remain the same (a number of search forms contained within tabbed panels). Your approach should focus specifically on:

  * Web Standards and good practices
  * Meeting the needs assistive technology users
  * Multi-device use

Your answer should describe both ***how*** you would do this and describe ***what*** specific features of HTML, ARIA, CSS and JavaScript you would use to achieve this.

### JavaScript

1. Given the HTML shown below write some JavaScript (you're welcome to use libraries) that will hide the first `<li>` that is clicked on. Any subsequent clicks should have no effect. Your approach should leverage event delegation.

```html
<body>
  <h1>DOM manipulation using event delegation</h1>
  <p>Choose a language to hide</p>
  <div>
    <h2>First set</h2>
    <ul>
      <li>HTML5</li>
      <li>CSS</li>
      <li><span class="highlight">JavaScript</span></li>
      <li>Ruby</li>
      <li>Django</li>
      <li><span class="highlight">React</span></li>
    </ul> 
  </div>
</body>
```

2. If you saw this in a Pull Request, what would your advice be:

  ```javascript
  Array.prototype.split = function(i) { // Adds split to all arrays
      return [this.slice(0, i), this.slice(i)];
  };
  ```

### CSS

1. What colour would each of the following elements be (Assume each pair of rules are targeting the same element). Explain your answer.
  ```css
  h1 {color: red;}
  body h1 {color: green;}

  h2.grape {color: purple;}
  h2 {color: silver;}

  html > body table tr[id="totals"] td ul > li {color: maroon;} // li has an id of answer
  li#answer {color: navy;}
  ```

2. Given the HTML below, write a CSS3 rule that will will prepend the text ‘Tel:’ to the third list item. You are not able to amend the HTML to achieve this.
  ```html
  <body>
    <ul>
      <li>JavaScript</li>
      <li>HTML</li>
      <li>Ruby</li>
      <li>Python</li>
    </ul>
  </body>
  ```

3. What changes would you suggest to make these CSS rules ready for a production environment?
  ```html
  <!DOCTYPE html>
  <html>
      <head>
      <meta charset=utf‐8 />
      <title>Test</title>
        <style type="text/css">
          #one { background‐color: #000; }
          .three { color: rgba(255,255,255,1); }
          div > span { border: 3px solid green; }
        </style>
      </head>
      <body>
        <div id="one">
          <div class="three">
            Hello <span>World!</span>
          </div>
        </div>
      </body>
  </html>
  ```

4. How would you style all links to 'gov.uk' domains differently to other links in an application?

### HTML

1. Review `test-html.html` within this repository. The HTML contains a number of errors and stylistic problems. Please describe errors that relate to HTML5. Do not:
    * Describe errors that are specific to XHTML, but which are not relevant to HTML5
    * Suggest stylistic changes that are not relevant to the specification

### Testing

1. What are **the key things you need to test for** on the front-end of digital services?

2. How do you approach testing the front end of applications?

### Best practices

1. Is this good quality code? Provide a brief justification of your answer.

  ```css
    <button
      type="button"
      onclick="document.getElementById('xyz').style.color='red';">
        Click Me
    </button>
  ```

2. Describe three ways to decrease page load time (answers may include perceived or actual load times)

3. Why is it generally a good idea to position CSS ```<link>``` elements between ```<head></head>``` tags and JS ```<script>``` elements just before ```</body>```? Do you know any exceptions?
