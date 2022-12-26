# Lesson 05: Details

## Context
* **Course:** Web Development
* **Main Objective:** Be able to update attribute, CSS properties, and classes of HTML elements.

## Warmup

Examine the attributes in HTML:
* the `href` in `<a href>`
* the `src` in `<img src>`

Examine the style properties in CSS:
* `color`
* `font-size`

Why do we have classes in CSS?
> Classes allow us to apply CSS to multiple HTML elements, even if they are not of the same type.

## Mini-lesson: Dom Details

### Explain:

* .attributeName allows us to get/set an attribute, like href or src
* .style.propertyName allows us to set a CSS property
  * Example: .style.color = "red"
  * Note: dash-case becomes camelCase
    * Example: margin-top becomes marginTop
* .classList
  * allows us to modify classes of a selected element:
    * .add()
    * .remove()
    * .toggle()

---

### Demo:

```html
<!DOCTYPE html>
<html>
    <head>
        <!-- Required meta tags -->
        <meta charset="utf-8">
        <meta name="viewport" content="width=device-width, initial-scale=1">

        <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0-beta1/dist/css/bootstrap.min.css" rel="stylesheet" />
        <!--<link href="style.css" rel="stylesheet" type="text/css" />-->
        <style>
            /* CSS */
            .pink-bg {
                background-color: pink;
            }
            
            .blue-bg {
                background-color: lightblue;
            }
            
            .large {
                font-size: 30px;
            }
            
            .light-padding {
                padding: 20px;
            }
            
        </style>
        
        <title>Details</title>
    </head>
    <body>
        <!-- HTML -->
        <p>Have you been <a href="http://jmap.org">here</a>?</p>
        <img src="https://i.imgur.com/HTXTKU7.jpg">
        
        <hr>
        
        <h1>Hello Human</h1>
        
        <hr>
        
        <p id="name" class="pink-bg">My name is Sniffles</p>
        <p id="food">I like to eat jello</p>
        <p id="activity1" class="blue-bg">I like to play tag</p>
        <p id="activity2" class="blue-bg light-padding">I like to take naps</p>
        
        <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0-beta1/dist/js/bootstrap.bundle.min.js"></script>
        <!--<script src="script.js"></script>-->
        <script>
            // JS
            
            // .attribute
            
            // get
            // console.log(document.querySelector('a').href);  // http://jmap.org
            
            // set
            document.querySelector('a').href = "http://mathbitsnotebook.com/";  // setting href to new address
            
            // get 
            // console.log(document.querySelector('img').src);   // https://i.imgur.com/HTXTKU7.jpg
            
            // set
            document.querySelector('img').src = "https://i.imgur.com/mC4Z62v.jpg";  // setting src attribute to new jpg address
            
            // CSS
            
            var greeting = document.querySelector('h1');
            greeting.style.color = "green";
            greeting.style.fontFamily = "Times New Roman";
            
            // .classList
            
            // get
            // console.log(document.querySelector('#name').classList);   // ['pick-bg']
            
            // add large
            document.querySelector('#food').classList.add('large');   // add classess
            
            // remove blue
            document.querySelector('#activity1').classList.remove('blue-bg');  // remove classes
            
            // toggle padding
            // if off, turn on, otherwise (it's on) turn off
            document.querySelector('#activity2').classList.toggle('light-padding'); // even toggle (if on, turn off; if off, turn on)
        </script>
    </body>
</html>
```


## Practice
Students can make a webpage and access/manipulate the attribute, css style property, and classes of a selected element.