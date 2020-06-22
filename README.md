# Design-your-own-Framework
This assignment consists of building a grid-based framework (similar to bootstrap) that includes some basic functionality to speed up the building process of a website.

[Live version](https://israel-laguan.github.io/Design-your-own-Framework/)

# Features

## Toggle Overlay

Try the button to toggle the FUN!

## Grid system

Built for column/row composition, really minimal grid system. In our opinion is a good thing to know when there are constrains using flex or grid (like coding for IE less than IE11), but a grid system dont beat `grid` or `flexbox` (maybe mixing `grid`+`flex`+`grid system`?). On the other side it was fun to make!

### Usage

You must have a parent with `wrapper` class, where you put elements to form a row:

```html
<main class="wrapper">
    <div id="element_1">
    <div id="element_2">
    <section id="element_3">
    <!-- Your rows here -->
</main>
```

You can specify the *width* of the row using a `container_<number>`, where `<number>` is an integer from _1_ to _12_. 

The grid have _12_ columns, and the sum of all `<number>`s must be equal or less than _12_; Then you have made a *row*:

```html
<main class="wrapper">
    <div class="container_6" id="element_1 row_1">
    <div class="container_6" id="element_2 row_1">
    <section id="element_3 row2">
    <!-- Your rows here -->
</main>
```

As the `container`s just make the *columns* you can add classes to style to your heart desire, thus achieving *Separation of concerns*:

```html
<main class="wrapper">
    <div class="style-me container_6" id="element_1 row_1">
    <div class="container_6" id="element_2 row_1">
    <section id="element_3 row2">
    <!-- Your rows here -->
</main>
```
> Note that `element_1` have a new class called `style-me`!

```css

.style-me {
  background-color: blue;
  height: 100px;
}
```

You can also define your own width but you will not align with the grid, so beware.

## Basic Responsiveness

Try to change the sizes from `760px` to `1200px` and note that the _columns_, the _overlay_ and the _grid system_ is working fine.

# Built With

* Flex and float
* BEM Naming convention
* SASS precompiler
* HTML5
* JS (for the demo only)

# Authors

* [Mario Dena](https://github.com/MarioDena).
<table style="width:100%">
  <tr>
    <td>
        <div align="center">
            <a href="./docs/img/photo.png" target="_blank" rel="author">
                <img src="https://avatars2.githubusercontent.com/u/36519478?s=460&v=4" style="border-radius: 10%; min-width: 100px;" alt="Israel Laguan's Photo" width="200px">
            </a>
            <h2>
                <a href="https://israel-laguan.github.io/" target="_blank" rel="author">
                    Israel Laguan
                </a>
            </h2>
        </div>
    </td>
    <td>
        <div align="center">
            <a href="mailto:israellaguan@gmail.com" target="_blank" rel="author">
                <img src="https://img.icons8.com/color/48/000000/message-squared.png" style="border-radius: 10%" alt="My GitHub" height="45px">
                <h3>
                    Email me to 
                    <a href="mailto:israellaguan@gmail.com">
                        israellaguan@gmail.com
                    </a>
                </h3>
            </a>
            <a href="https://www.linkedin.com/in/israellaguan/" target="_blank" rel="author">
                <img src="https://img.icons8.com/color/48/000000/linkedin.png" alt="My Linkedin" height="45px">
                <h3>
                    Connect to my Linkedin
                </h3>
            </a>
            <a href="https://github.com/Israel-Laguan" target="_blank" rel="author">
                <img src="https://img.icons8.com/color/48/000000/github--v1.png" 
			style="border-radius: 10%" alt="My GitHub" height="45px"
		>
                <h3>
                    Check my GitHub Profile
                </h3>
            </a>
        </div>
    </td>
  </tr>
</table>

# License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
