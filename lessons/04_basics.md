# Lesson 04: Basics

## Context
* Course: Web Development
* Main Objective: Introduce students to the DOM and to select and update content.

## Warmup
What do you notice about the image?
<a href="https://upload.wikimedia.org/wikipedia/commons/thumb/5/5a/DOM-model.svg/1200px-DOM-model.svg.png" target="_blank"> Dom Tree</a>

## Mini-lesson: DOM Basics

### Explain:
* inspect/console by using ctrl-shift-j
* Dom is a tree of node. This is how computer represents a webpage in its memory. HTML content cannot be changed by javascript, but
the live elements can be accessed and manipulated without modifying the html content. When a webpage is refreshed, the content is reset.
* `querySelector()` selects an element specified by id or the first of a group of selected elements.
* `.innerHTML` can be used for getting content, setting content, or adding to the content (concetenating)

---

### Demo:

```html
<!DOCTYPE html>
<html>
<head>
    <title>lesson 4</title>
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
    <h2 id="correctAnswer">Kinematics Q</h2>
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
    <script>
        var myh1 = document.querySelector('h1'); // will select <h1>Physics Jun 2022 Regents Exam</h1>
        console.log(myh1);
        var myAns = document.querySelector('#correctAnswer'); // will select <h2 id="correctAnswer">Kinematics Q</h2>
        console.log(myAns);
        console.log(myAns.innerHTML);
        myAns.innerHTML = "Mechanics Question";
        console.log(myAns.innerHTML);
        myAns.innerHTML += " on Kinematic Motion";
        console.log(myAns.innerHTML);

    </script>

    

</body>
</html>
```

## Practice
Students can make their own examples of using querySelector and innerHTML to access and manipulate html content.

```html
3) A battery-powered electric motor is used to cause
the wheels of a toy car to rotate. In this motor,
there is a conversion of
(1) mechanical energy to electric energy
(2) electric energy to chemical energy
(3) thermal energy to electric energy
(4) electric energy to mechanical energy

4) A projectile is launched horizontally from a height
of 65 meters with an initial horizontal speed of
35 meters per second. What is the projectile’s
horizontal speed after it has fallen 25 meters?
[Neglect friction.]
(1) 22 m/s (3) 41 m/s
(2) 35 m/s (4) 280 m/s
```

## Source
[01_basics lesson](https://github.com/hunter-teacher-cert/currdev_unit_plan-jsdom/blob/main/lessons/01_basics.md)