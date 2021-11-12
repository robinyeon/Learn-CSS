## Transitions
- Make a change from one state to another.
- **Transition should be on the root element**, not on the state. (e.g. `a` not `a:hover`)
- e.g. `transition: background-color 10s ease-in-out, color 5s ease-in-out` or `transition: all 5s ease-in-out`

### [Useful website](https://matthewlein.com/tools/ceaser)
- `cubic-bezier()` allows you to make your own animation

<br/>

## Transformations
fyi) border-radius:50% === circle     
- e.g. `transform: rotateY(35deg)`, `transform: translate(300px)`
- Don't use `translate`(옮기다) for margin or padding. It's for moving the element without modifying the box of the other elements. (3D stuff)

<br/>

## Animations
Use when you want to animate the element without a state like `:hover` or play the animation all the time.

### 1. from to
```
<style>
@keyframes nameOfTheAnimation{
  from {
    transform: rotateX(0deg);
  }
  to {
    transform: rotateX(360deg);
  }
}

img {
  animation: nameOfTheAnimation 5s ease-in-out infinite;
}
</style>
```

## 2. %
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

## Reminder
<img src="https://user-images.githubusercontent.com/85475577/141408576-c9b45daf-0693-4d9f-8016-999c7d440ff1.jpeg" alt="note" width="500px"/>
