## How to add CSS to HTML
1. Inline CSS: write CSS code inside a HTML file.     
e.g. ```<head> <style>Write CSS code here </style> </head>```
2. External CSS: create a CSS file.
e.g. ```<link href="style.css" rel="stylesheet" />```

<br/>

## CSS Basic
```
selector {
  property: value;
}
```
- property name should not includes ``` ```(blank space) or ```_``` or ```/```

#### fyi) [attribute vs property](https://medium.com/hexlant/attribute-%EC%99%80-property-%EC%9D%98-%EC%B0%A8%EC%9D%B4-c6f1c91ba91)
- attribute는 html 문서 안에서의 정적인(바뀌지 않는) 속성 그 자체를 의미, property는 html DOM 안에서 동적인(바뀌는) 속성(또는 그 값)을 의미   
- e.g. ```<div class= ‘my-class’></div>```
- 즉 html 문서 안에서는 ```class```가 attribute를 의미하지만 html DOM 안에서는 property를 의미

<br/>

## Cascading: one after another
- CSS codes are applied from top to bottom
- If you wrote same tags and applied different values, the one in the bottom would be applied.

<br/>

## blocks and inlines
- Block: do not allow anything next to them. (e.g. div, p, section, header)
- Inline: means 'in the same line.' Inline allows elements to be next to them. (e.g. span, link, image)
- Block and Inline are  by using ```display: block or inline```.

### Differences
- Block is simply a box. So 'margin, padding, border' avail.
- Inline: is not a box so it **does not have width and height** 
  - Padding: top & bottom, left & right all avail.
  - Margin: only left & right avail. 
  
<br/>

## margin
- Margin is a space from the border of the box to the outside.
- *Collapsing margins*: Because of the box's border is also same as the outter box's border then their margin becomes one.
  - Don't think to deep about collapsing margins just realize it happens.

## padding
- Padding is a space from the border of the box to the inside.

## border
- Border is a border of the box. (e.g. ```border: 2px solid black```)
- Border could be applide on both inline and blcok. 

<br/>

## class
- ```id``` should be unique so we need sth as a pointer which does not need to be unique => ```class```
- Class don'y need to be unique. It can be shared and one tag can have many classes at the same time.

<br/>

## inline-block
- Don't use this often because it's old and has many problems.
  - problem(1) space btw
  - problem(2) no specific forms
  - problem(3) does not support responsive design

<br/>

## flex
### 1. If you want to move children, talk to parents.
- 바꾸고자하는 태그의 부모태그를 ```display: flex```로 만들기
- then you can unlock many properties such as ```justify-content```

### 2. flex's properties
- ```justify-content``` for main-axis(horizontal)
- ```align-items``` for cross-axis(vertical)
- ```flex-direction: column or row``` : could flip the situation
- ```flex-wrap: nowrap```: everything on the same line
- flexbox take the property ```width``` as the initial size but then it may changes.
