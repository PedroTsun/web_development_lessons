# Lesson 03: CSS

## Context
* **Course:** Web Development
* **Main Objective:** To show understanding of the reasons for CSS by selecting specific elements on a webpage

## Warmup
Would you know how to change color of text in html?

## Mini-lesson: CSS

### Explain:
* CSS stands for cascade style sheet
* To change color of a text, we can use an in-line style attribute and set the color property
  * `<h1 style="color:red"> Lesson 3 </h1>`
* To select an **individual** htmml element, like <p>, we use an id selector
  * `<p id="intro-para">I am learning about purpose of CSS ... </p>`
* To select a group of html elements, like a few <p>, we use a class identifier
  * `<p class="important-para">This CSS technology makes website building an amazing experience</p>`

---

### Demo:

Imagine you are to change the color of all heading h1 in hundreds of webpages.

```html
<!DOCTYPE html>
<html>
<head>
    <title>lesson 1</title>
    <style>
        #correctAns {
            background: green;
        }
        .keyQuestion {
            color: orange;
        }
    </style>
</head>
<body>
    <h1 style="color:red;">Physics Jun 2022 Regents Exam</h1>
    <p class="keyQuestion">
    1) Which terms identify two scalar quantities?
    <ol>
        <li> force and acceleration</li>
        <li> impulse and distance </li>
        <li> mass and velocity</li>
        <li id="correctAns"> energy and time</li>
    </ol>
    </p>
    <div class="keyQuestion">
    <p>
    2) A motorcyclist, initially traveling east at 15 meters
    per second, accelerates uniformly at a rate of
    3.0 meters per second squared east to a velocity
    of 21 meters per second east. How far does the
    motorcyclist travel while accelerating?
    <ol>
        <li>1.0 m</li>
        <li>2.0 m</li>
        <li>36 m</li>
        <li>72 m</li>
    </ol>
    </p>
    </div>
</body>
</html>
```

### Practice
Make a webpage with mulitple paragraphs. Use CSS to control the style property of many elements from a single place in the head section of your html file.