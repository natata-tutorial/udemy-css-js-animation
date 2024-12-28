# Creative Advanced CSS & JavaScript Animations - 150 Projects
files for [Creative Advanced CSS & JavaScript Animations - 150 Projects](https://www.udemy.com/course/css-animation-transitions-and-transforms-creativity-course/)

## CSS Transitions

change element properties smoothly in some period of time

### transition-timing-function
[MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/transition-timing-function)
- ease : slow-fast-slow
- linear : equal
- ease-in : slow-fast
- ease-out : fast-slow
- ease-in-out : slow-fast-slow

```css
 transition: background-color 3s ease-in-out 1s, color 2s ease 4s, border-radius 4s eaase-out 6s;
 transition: all 3s ease-in-out 2s;

 ```


## CSS Transforms

cahnge elements - size, shape, position

```css
	img{
		transotion: transform 2s;
		transform-origin: top; // default pivot point - center center
	}
	img:hover{
		transform: translate(X, Y); 
	} 
 ```

 transform-origin defines the point around which a transformation is applied
 ```css
 transform-origin: top; // top center
 transform-origin: bottom right;
 transform-origin: 50px 50px;
 transform-origin: 30% 80%;
 ```

 the order of transformations is important

 ```css
  transform: rotate(45deg) translateX(180px);
  transform: translateX(180px) rotate(45deg); // result is different
 ```

### translate 
[MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/transform-function/translate)

 ```css
 transform: translate(X, Y); // move diagonale
 transform: translateX(100xp); // move right
 transform: translateY(-100px); // move top
 ```

### scale
[MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/transform-function/scale)

```css
 transform: scale(width, height); 
 transform: scale(2);// increase width, height
 transform: scaleX(.5); // decrease width
 transform: scaleX(-1); // flips horizontally
 transform: scaleY(2); // increase height
 ```

 ### rotate
[MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/transform-function/rotate)

```css
 transform: rotate(90deg); //clockwise
 transform: rotate(-90deg); //counter clockwise
 transform: rotate(3.149rad); 
 transform: rotate(-0.25turn); 
 ```

 ### skew
[MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/transform-function/skew)

```css
 transform: skewX(90deg); //to the left
 transform: skewY(-90deg); //to the top
 transform: skew(3.149rad); 
 transform: skew(-0.06turn, 18deg);
 ```
