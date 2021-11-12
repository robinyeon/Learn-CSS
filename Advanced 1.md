***WIP***

## Transitions
animate a chage from one state to another
abrupt to vague
apply to the element without the state. not a:hover, on a. **should be on the root**. on the element, not on the state.
transition: background-color 10s ease-in-out, color 5s ease-in-out;
or 
transition: all 5s ease-in-out;

ease-in-out > how to animate change
[Useful website](https://matthewlein.com/tools/ceaser)
cubic-bezier() make my own animation

transition happens when you have a property that changes btw states.
most common way is going to be 'all'

## Transformations
border-radius:50% === circle
transform: rotateY(35deg) or transform: translate(300px)
touching pixels. do not use 'translate(옮기다)' for margin or padding. 3d stuff. 
wanna move the element without modifying the box of the other elements
transformation does not affect other box elements.

## Animations
without state like :hover. playing all the tiem > animations
1. 
```
<style>
@keyframes nameoftheanimation{
  from {
    transform: rotateX(0deg);
  }
  to {
    transform: rotateX(360deg);
  }
}

img {
  animation: nameoftheanimation 5s ease-in-out infinite;
}
</style>
```
2.
```
<style>
@keyframes nameoftheanimation{
  0% {
    transform: rotateY(0deg);
  }
  50% {
    transform: rotatey(180deg) translateY(100px);
  }
  100% {
    transform: rotateY(0deg) translateY(0px);
  }
}

img {
  animation: nameoftheanimation 5s ease-in-out infinite;
}
</style>
```



















