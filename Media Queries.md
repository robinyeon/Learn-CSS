## Media Query
- Telling the browser to show specific CSS on specific screen size.
- With only CSS, detecting the users' screen size who's visiting your website.
- `portrait` vertical mode, `landscape` horizontal mode.

<br/>

```
@media screen and (max-width: 400px) {
 /* CSS code here*/ 
}
```
- means "if these conditions are true then execute these CSS."
- In the above code: if the screen have less than 400px, then shows CSS code inside {} curly bracket.

<br/>

### You can change conditions:
```
@media screen and (min-width:100px) and (max-width: 400px) {
  /* CSS code here*/ 
}
```

<br/>

### For landscape mode:
``` and (orientation: landscape)```

<br/>

## Media type 
`@media mediatype and (...){ }`
- mediatypes are normally `screen` or `print`
- `print` is for print mode. (cmd+p)
