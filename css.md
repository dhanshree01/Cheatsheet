### CSS BASICS
#### 1. Style tag
```html
<style>
  button {
    background-color: red;
    color: white;
    border: none;
    height: 36px;
    width: 105px;
    border-radius: 2px;
    cursor: pointer;
  }
</style>
```
### HOVERS, TRANSITIONS, SHADOWS
#### 1. Hover (pseudo class) : The styles mentioned in the hover pseudo class gets applied only when the object is hovered. Opacity fades out an element and takes values between 0-1.
```css
.subscribe-button:hover {
    opacity: 0.3; 
  }
```
#### 2. Active (pseudo class) : The styles mentioned in the active pseudo class gets applied only when the object is clicked.
```css
.subscribe-button:active {
    opacity: 0.5;
  }
```
#### 3. Transition (property) : Allows to change property values smoothly, over a given duration. It takes two values what to transition and duration of transition. Always add transition property to base css style.
```css
.subscribe-button {
    background-color: rgb(200, 0, 0);
    color: white;
    transition: opacity 0.15s,
      background-color 0.15s,
      color 0.15s;
  }
.subscribe-button:hover {
    opacity: 0.8;
    background-color: rgb(41, 118, 211);
    color: white;
  }
 ```
#### 4. Shadow (property) : It creates shadow of an element. Takes four values horizontal, vertical, blurr, color.
```css
.tweet-button:hover {
    box-shadow: 5px 5px 10px rgba(0, 0, 0, 0.15);
  }
```
### CHROME DEVTOOLS AND CSS BOX MODEL
#### 1. Margin (property) : Spacing on the outside of the element.
```css
.tweet-button {
    margin-left: 8px;
    margin-bottom: 8px;
  }
```
#### 2. Padding (property) : Spacing on the inside of an element.
```css
.tweet-button {
    padding-right: 8px;
    padding-top: 8px;
  }
```
#### 3. Vertical-align : Aligns every element together.
```css
.tweet-button {
    vertical-align: top;
  }
```
### TEXT STYLES 
```css
.video-stats {
    font-family: Arial;
    font-size: 14px;
    font-weight: bold;
    line-height: 24px;
    text-align: center;
    text-decoration: underline;
  }
```
### IMAGES AND TEXT BOX
#### 1. Images 
```css
img {
    border-radius: 50%;
    border: 1px solid #ddd;
    padding: 5px;
    width: 150px;
  }
```
### CSS DISPLAY PROPERTY
#### 1. Block element : Takes up the entire line in the container (p, div)
#### 2. Inline block element : Only takes up as much space as needed
#### 3. Inline element : Appear within a line of text (strong)
```css
.thumbnail {
    display: inline-block;
   }
```
### The DIV element
```css
.video-preview {
    display: inline-block;
  }
<div class="video-preview">
    <img class="thumbnail" src="thumbnails/thumbnail-1.webp">
</div>
```
### NESTED LAYOUTS TECHNIQUE
![Screenshot (58)](https://user-images.githubusercontent.com/85294480/210135448-a7c328b0-a0da-4c03-b89d-83d90d1eb4d0.png)
![Screenshot (56)](https://user-images.githubusercontent.com/85294480/210135519-5bfce6f0-bda3-4d04-899d-15cb5b84767c.png)
#### Use google drawings for creating nested layouts.
### CSS GRID
#### A grid is a layout that has rows and columns. It makes it easier to design web pages without having to use floats and positioning.
```html
<div style="
      margin-top: 30px;
      display: grid;
      grid-template-columns: 1fr 1fr 1fr;
      column-gap: 20px;
      row-gap: 40px;
    ">
      <div style="background-color: lightblue; height: 200px;">1fr</div>
      <div style="background-color: lightpink; height: 200px;">1fr</div>
      <div style="background-color: lightblue; height: 200px;">1fr</div>
      <div style="background-color: lightpink; height: 200px;">1fr</div>
      <div style="background-color: lightblue; height: 200px;">1fr</div>
      <div style="background-color: lightpink; height: 200px;">1fr</div>
    </div>
```
![Screenshot (60)](https://user-images.githubusercontent.com/85294480/210135953-d28d0e00-26be-4210-b82c-7e5c5cf22857.png)
### FLEXBOX
#### Flexbox is similar to CSS grid but it's more flexible.
```html
<div style="
      margin-top: 30px;
      height: 70px;
      border-width: 1px;
      border-style: solid;
      border-color: gray;
      display: flex;
      flex-direction: row;
      justify-content: center;
    ">
      <div style="
        background-color: lightblue;
        width: 100px;
      ">100px</div>
      <div style="
        background-color: lightpink;
        width: 100px;
      ">100px</div>
      <div style="
        background-color: lightblue;
        width: 100px;
      ">100px</div>
    </div>
```
![Screenshot (62)](https://user-images.githubusercontent.com/85294480/210136430-a10fb216-35e8-4503-b473-2b1e8a7206ce.png)
```html
<div style="
      margin-top: 30px;
      height: 70px;
      border-width: 1px;
      border-style: solid;
      border-color: gray;
      display: flex;
      flex-direction: row;
      justify-content: space-between;
    ">
      <div style="
        background-color: lightblue;
        width: 100px;
      ">100px</div>
      <div style="
        background-color: lightpink;
        width: 100px;
      ">100px</div>
      <div style="
        background-color: lightblue;
        width: 100px;
      ">100px</div>
    </div>
```
![Screenshot (62)1](https://user-images.githubusercontent.com/85294480/210136474-7ace9857-4286-49ed-800e-70c8018b3f0d.png)
```html
<div style="
      margin-top: 30px;
      height: 70px;
      border-width: 1px;
      border-style: solid;
      border-color: gray;
      display: flex;
      flex-direction: row;
      justify-content: space-between;
      align-items: center;
    ">
      <div style="
        background-color: lightblue;
        width: 100px;
      ">100px</div>
      <div style="
        background-color: lightpink;
        width: 100px;
      ">100px</div>
      <div style="
        background-color: lightblue;
        width: 100px;
      ">100px</div>
    </div>
```
![Screenshot (62)2](https://user-images.githubusercontent.com/85294480/210136524-0ee3f19e-de0e-4b6f-a2b1-14379a521398.png)
### NESTED FLEXBOX
#### flex-shrink: 0; -> don't shrink
#### width: 0; -> shrink
### CSS POSITION
#### The position property specifies the type of positioning method used for an element (static, relative, fixed, absolute or sticky).
#### 1. Static : Default position 
#### 2. Relative : The element is positioned relative to its normal position.
#### 3. Fixed : The element will always stay in the same place even if the page is scrolled.
#### 4. Absolute : Element is positioned relative to the nearest positioned ancestor. If an absolute positioned element has no positioned ancestors, it uses the document body, and moves along with page scrolling.
#### 5. Sticky : Element is positioned based on the user's scroll position.
#### 6. z-index : The z-index property specifies the stack order of an element. An element with greater stack order is always in front of an element with a lower stack order.

### MORE CSS FEATURES
#### 1. Media query
#### 2. Inheritance
#### 3. Semantic elements
