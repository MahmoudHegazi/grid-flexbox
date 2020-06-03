# grid-flexbox
grid and flex box example 

# layout1:
<img src="mylayout1.PNG">

# layout2:
<img src="layout2.PNG">

# layout3:
<img src="layout3.PNG">


```html

.layout {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  // same as:
  // grid-template-columns: repeat(3, 1fr);
  grid-gap: 8px;
}
.child {
  min-height: 100px;
  background: orange;
  line-height: 100px;
  text-align: center;
}

```
