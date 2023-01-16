| Some extra efforts
| See corresponding files

<div>

<img src="./design/Screenshot (64).png" alt="image of neumorphism" class="img1" width="40%"/> <img src="./design/Screenshot (65).png" alt="image of glassmorphism" class="img1" width="40%"/>

</div>

# Think about the structure \^\_\_\_\_\_\^

|  Take a look at our design

![nft card design desktop preview](design/desktop-design.jpg){width="512"}

    <main>
    <figure><figure> for img
    <h1>
    <p> 
    <ul> to wrapp two items with flex
    <li></li>
    <li></li>
    </ul>
    <div>
     for bottom section
    </div>
    </main>

## How we'll manage section after figure?🤷‍♂️

-   Break it down to

`'<h1></h1>`

`<p></p>`

`<ul>`

`<li><img><span></span></li>`

`<li><svg> and <span> </li>`

`</ul>'`

**Yaay 😁**

-   Now how to style this

Imagine the flex box structure

![Flex-box and grid layout of design](design/layout.png){width="523"}

-   but how to achieve👂

`ul {`

`margin: 25px auto;`

`display: flex;`

`justify-content: space-between;`

`align-items: baseline;`

`}`

`ul li {`

`list-style: none;`

`display: flex;`

`align-items: center;`

`gap: 5px;`

`}`

-   Okay then, what about horizontal line 👊❓

    `Using <hr>`

    ## Profile part

    what in my mind is -----

    ------------------------------------------------------------------------

    ```{=html}

    <div class="profile">
            <img src="images/image-avatar.png" alt="Profile photo of user." />
            <span>
              <span class="credit">Creation of</span>
              <span class="uname">Jules Wyvern</span>
            </span>
          </div>
    ```

### Flex properties

1.  `.profile {`

    `margin: 25px auto;`

    `display: flex;`

    `align-items: center; /* to align items vertically*/`

    `}`

`.profile img {`

`height: 35px;`

`width: 35px;`

`border: 1px solid var(--White);`

`border-radius: 50%;`

`margin-inline-end: 15px;   Same as margin-right`

`}`

### Secret of image preview feature

![active state of design on web](design/active-states.jpg){width="512"}

1.  To achieve this feature

    `<figure>`

    `<img class="main"/>`

    `<div class="preview">`

    `<img class="hoverimg" />`

    `</div>`

    `</figure>`

2.  and now

<!-- -->

    `img { height: 100%;  width: 100%;} Both images will take all the space`

3.  Hiding icon with opacity 🦸

<!-- -->

    `.preview {`

    `position: absolute;`

    `top: 50%;`

    `left: 50%;`

    `transform: translate(-50%, -50%);`

    `opacity: 0;`

    `display: flex;`

    `justify-content: center;`

    `align-items: center;`

    `height: 100%;`

    `width: 100%;`

    `}`

4.  That blueish effect 👌

<!-- -->

    `.preview:hover { background: var(--cyan); opacity: 0.5;}`

-   We are done with main techniques to complete this challenge🐬

------------------------------------------------------------------------
