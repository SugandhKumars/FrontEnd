## About CSS

- How you can link your CSS File to your HTML File?

- We have mainly three ways ro link our Css file to HTML file
  - InLine Css
  - By using Style tag
  - Using link tag to link a style file

### Units in CSS

-There are mainly ive units we have to learn in css

- px
- %
- vh
- vw
- em
- rem

  - ## px
  - It is straight forward it wil be denoting the pixels in the screen.
  - ## %
  - it will take the height or width with respect to its parent element heigth or width in percentage.
    - For Ex- if a parent div has a height of 100px and inside that div we have a element and we gave it height to be 50% then it will take 50px height.
  - ## vh and vw
  - It stands for Viewport Height and Viewport Width. so It will be take the space according to the Size of the screen .

  - ## em
  - it will take the value of it value or its parent value

    - for example : - if a div is having a font-size of 12px and we have it height to be 2 em then it will take the width to 24 px and Similary for its parent Element also.

  - ## rem
  - It will take the value of the root element
    - for Example : - if we set the font size of html to be 10px and when ever we use rem then it will be take value from the root . Like if write 2rem that means 20px.

### Max width and Max Height

- ## Max-Width and Min-Width
  - So what we understand when we say max height or max width. when ever we use max height it means that is the maximum limit that the height can go up to no matter up gave what value of height , if you give the height value which is greater than the max value then it will take the max height not the value that you given as height but if you give the vakue of height less than the max height then it will work as usual .
  - The Similary it will for max-width
  - In case of min-width or min-heigth it will work similarly but the catch is this time it will be minimum value thant not going to change it means you give the value which is greater thean the min value it will work properly but if give value which is less than the min value then it will take the min value.

### Padding And Margin

- Padding means the space inside the border .
- Margin means the space outside the border.

### Border

- Border means the border space is between padding and margin.

### Display

- ## Mainly there are three type of Display Property i.e.

  - block
  - inline
  - inline-block

- ## Block
  - So what we understand if a div or any tag having the display property as block , that means it will take the whole space no element can be in its right or left .
- ## Inline
  - Inline property means it will take the space that is required fot it.
  - One more thing that we can not set height and widtht to the inline element.
- ## Inline-Block
  - Inline-Block is that property when we want that the element should follow the inline property and we can set the height and width of the element.

### Position

- The Default value of the position id Static.

- Mainly we study about the following position properties
  - Absolute
  - Relative
  - Fixed
- ## Position : Absolute
- if we set position absolute to any element it comes above every element and it can move any where according to the given dimension.
  for Ex-
  <div style = "background-color : green ; width : 250px; padding: 10px;"> 
    <p style="position: absolute; top:20%; left:50%; right:0; width: 100px; height: 100px; background-color: red;"></p>

    <p style=" width: 120px; height: 120px; background-color: yellow;"> </p>
    <p style=" width: 120px; height: 120px; background-color: blue;"> </p>
  </div>

  - In the above Example first element position is absolute so it can be move anywhere according to its position value and the value is relative to the main page ( means it will be move relative with page like we give from top 20% then it will be move 20 % with relate to the page not with its parent element ).
  - Using absolute position we can move it outside its parent div also.

- ## Position : Relative
- Position Relative lets Understand this by an example . Like in postion abslute we can move the element anywhere in the main body of the html . But using Relative we can assure that it will move relative to its parent
- Like if we give from top 20% then it will take the 20% from its parent not with the page.

<div style="background-color : green ; width : 250px; padding: 10px; position:relative"> 
<p style=" position:absolute; top:20%; left:50%; width: 100px; height: 100px; background-color: blue;"></p>
<p style="  width: 100px; height: 100px; background-color: red;"></p>
<p style=" width: 100px; height: 100px; background-color: red;"></p>
</div>

- ## Fixed
- it let's you fixed any element tot the body.

### BackGround

- ## Background Image
  - Let's seee an Example
   <div style=" width : 300px ; height : 300px ; background:url(https://images.unsplash.com/photo-1709319815910-517700bfcbb7?q=80&w=1374&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D); background-size : cover; background-position : center"  >
  </div>
- ## Linear-Gradient using Background
  - Example
  <div style=" width : 300px ; height : 100px ; background:linear-gradient(to right, orange , red ); background-size : cover; background-position : center"  >
    </div>

### Flex

- How flex is working let's understand !!

  - Flex is always pass to the parent element not to the child element . When we pass flex to an parent then all the child element comes beside each other .
  - The Default value of the flex is row .

    - lets see an example
    <div style="background-color:yellow ;width:250px; padding:10px; display : flex; justify-content : center;">
    <p style="background-color:red; width:50px; height : 50px; margin:10px
    "></p>
    <p style="background-color:red; width:50px; height : 50px ; margin:10px
    "></p>
    <p style="background-color:red; width:50px; height : 50px; margin:10px
    "></p>
    </div>

    - On Two axis whrere the flex is working
      - Main Axis
      - Cross Axis
    - When flex direction is row then the x -axis is main axis and y-axis is cross axis .
    - Similarly with the flex-direction column ,
      then the x-axis is cross axis and y-axis is main axis.

    ### Psuedo-Elements

    - ::before
    - ::after
    - ::first-line
    - ::selection
      - Lets use them one by one
    - ::before
      - Using this we can add content before the element
    - ::after
      - Using this we can add content after the element
    - :: first-line
      - using this we can change the any property of thefirst line of any paragraph
      - And it is completly dianamic means when we increase or decrease the screen size it will be apply on those which are on the first line of the paragraph.
    - ::selection
      - Using Selection we can add the functionality of change the property of the element when we select it.
        - For ex : - we can add it to element when we select the element so it will be change the colur of it .

### Psuedo-Classes

- :hover
- :active
- :focus
- nth-child(n)
  - Lets Understand all of them onee by one what are they doing.
    - :hover
      - it use to change the property of an element on hovering on the element
    - :active
      - it is use to change the prperty of the element when we click on the specific element.
    - :focus
      - it is mostly use in the input tag , so focus means in input tag is when we click on the input tag inside to type something that is called the focus. On that specific state we can change its property by using focus.
    - nth-child(n)
      - It is use to change the property of the element on the basis of the position within their parent element.
      - for ex -  
        Let's assume we have 6 p tag and we want to change theproperty of the 2nd p tag so we can do it using this p:2nd-child{any property}
        OR lets say you wanna change the property of each 3rd element so you can simply do it p:nth-child(3n){any property} , After this it will chnage the property of every third element .

## Difference between Psuedo-Elements and Psuedo-Classes

    - Psuedo-classes targets states or characterstic of elements while psuedo elemets targets specific parts of the elements content or generate additional content.

### GRID IN CSS

- It is also applied on only on the parent Element
- By using grid we can handle 2D .
- Let's take an example : -
<div style = "display : grid ; grid-template-columns: 20%  50%  30%;

">

<div style = " height: 100px; background-color : blue;">20%</div> 
<div style = "height: 100px; background-color : green">50%</div> 
<div style = "height: 100px; background-color : Red">30%</div>
 </div>
