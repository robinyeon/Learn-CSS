telling the browser 'if the screen size is this big, show this css'
with only CSS, detect size of the screen of the person looking at your website.
portrait(폰세로), landscape(폰가로)
```
@media screen and (max-width: 400px) {
  
}
```
if the screen have less than 400px, then shows CSS code inside {} curly bracket



```
@media screen and (min-width:100px) and (max-width: 400px) {
  div {
  
  }
}
```
can change conditions
``` and (orientation: landscape)``` 폰가로일때만 적용되는 조건

if these conditions are true then execute these CSS





media type 
@media mediatype and (...) and ...
mediatype normally `screen` or `print`
