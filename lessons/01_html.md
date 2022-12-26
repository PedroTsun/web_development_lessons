# Lesson 01: HTML

## Context
* **Course:** Web Development
* **Main objective:** Introduce students to writing a basic html webpage

## Warmup
* How do you save and share information?

## Mini-lesson: **HTML Basics**

### Explain:

* HTML is a layout language that allows people to communicate with browsers on what contents to display
* HTML uses opening and closing tags to designate the kind of content between the tags
* A webpage has a set of html tags enclosing it.
  * Within the webpage, there is a head section enclosed in a set of head tags
  * Following the head section, there is a body section enclosed in a set of body tags  
* There are many handy elements in HTML
  * Heading element is denoted by heading tags like h1. The size goes from 1 to 6.
  * Paragraph element is denoted by p tags.
  * List element is denoted by a ul, ol, and li tags
  * link element is denoted by a tag, which stands for anchor
  * image element is denoted by img tag

---

### Demo:

```html
<!DOCTYPE html>
<html>
<head>
    <title>lesson 1</title>
</head>
<body>
    <h1>Physics Jun 2022 Regents Exam</h1>
    <p>
    1) Which terms identify two scalar quantities?
    <ol>
        <li> force and acceleration</li>
        <li> impulse and distance </li>
        <li> mass and velocity</li>
        <li> energy and time</li>
    </ol>
    </p>
    <br>
    <hr>
    <br>
    <br>
    <img src="https://kb.rspca.org.au/wp-content/uploads/2018/11/golder-retriever-puppy.jpeg" alt="A golden retriever puppy">
    <br>
    <!-- <br> -->
    <a href="https://www.edx.org/cs50"> cs50 courses</a>
    

</body>
</html>
```

## Activity

Students can write a webpage on a local computer to display a regents question.

```html

<p>2) A motorcyclist, initially traveling east at 15 meters
per second, accelerates uniformly at a rate of
3.0 meters per second squared east to a velocity
of 21 meters per second east. How far does the
motorcyclist travel while accelerating?
(1) 1.0 m (3) 36 m
(2) 2.0 m (4) 72 m
</p>
```

## Additional Online Resource

* [Khan Academy HTML/CSS](https://www.khanacademy.org/computing/computer-programming/html-css)
* [CS50W html](https://youtu.be/zFZrkCIc2Oc)
* [Decrypted By Us: HTML & CSS Basics for Beginners](https://youtu.be/JVwYlC9hp7A)

