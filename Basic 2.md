## Fixed
```position: fixed```
- Stays in the initial position
- But can change the position by adding properties ```top, bottom, left, right```
- Because it's going to be on the completely defferent layer. On the top of the every layers.
- e.g. Chatting button on websites.

<br/>

## Relative, Absolute
'슬기로운 백신생활' 메인페이지 적용 이론
### ```position: static```(default)

### ```position: relative```
- then write down for example: ```top: 10px```, ```left: -5px```.
- Change the position based on where it starts(from the place where the element starts).
- e.g. Moving a small box div inside a parent div area.

### ```position: absolute```
- Absolute looks for the closest relative parent tag.
- ```<body>``` is going to be a parent if there's no ```position: absolute``` near.

<br/>

## Pseudo selectors 
```
div: last-child {
    color: tomato;
}
```
- Using pseudo selectors is much better than making tons of ids or classes.
- e.g. ```first-child```, ```last-child```, ```nth-child(2)``` = ```nth-child(even)```, ```nth-child(n+1)```, etc.

<br/>

## Combinators
```
<div>
    <span>hello</span>
    <p> Laphoo is my dog. He is the cutest dog in the world. But I wish he pee a little
        bit less than usual when I'm busy. <span>Laphoo</span>
    </p>
</div>
```
- ```div span``` : to all spans inside the div.
- ```div > span```: to only a direct child.
- ```p + span```: to span immediately next to p(siblings).
- ```p ~ span```: to span next to p, they don't need to be direct.

<br/>

## Attribute selectors
For tags with an attribute ```type="password"```, you can apply CSS like: ```input[type="password"]```      

### tilde ```~```
```
input[placeholder~="name"]{
  <!-- placeholder에 'name'을 포함하는 attribute를 가진 모든 input에 적용됨 -->
}
```

<br/>

## States
- ```button: active```: While clicking
- ```button: hover```
- ```button: focus```: Literally a focused one. Could be selected from keyboard. On focused.
- ```button: visited```: Only applies for a link ```<a>```. Activate visited(clicked) anchor.
- ```button: focus-within```: An element might have a child with ```focus```. Any child inside the element get focused, apply CSS to a parent.
- Combine for example: ```form:hover input { }```

<br/>

## Pseudo elements
```::placeholder```: apply css on placeholders      
```::selection```: highlighter          
```::first letter```, ```first-line```, etc.

<br/>

## Colors and variables(cusotm property)
### Colors
1. hexadecimal color #000000
2. rgb(0, 0, 0)
3. rgba(0, 0, 0, 0) : alpha for transparency

### Saving colors to the variable
```
:root {
    --main-color: #0000000;
    --default-border: 1px solid var(--main-color);
 }
 
 p{
    background-color: var(--main-color)
 }
 a {
    color: var(--main-color)
 }
```
