

| Anchor | details             | Typora | VsCode | GFM  |
| :----- | ---------------- | ------ | ------ | ---- |
| 1      | <a ,id ,<href    | ✗      | ✓      | ✓    |
| 2      | <a ,name ,<href  | ✓      | ✗      | ✓    |
| 3      | <span,id,<href   | ✗      | ✓      | ✓    |
| 4      | <span,name,<href | ✓      | ✗      | ✓    |
| 5      | <a,id,[](#       | ✗      | ✓      | ✓    |
| 6      | <a,name,[](#     | ✓      | ✗      | ✓    |
| 7      | # header [](#    | ✓      | ✓      | ✓    |

* With my test on System Win10 VsCode-1.44.2，Typora-0.9-86.
* Test 1,2 is a group  a,Test 3,4 is group b, Test 5,6 is another group c, the difference betweent group  is 'id' and 'name', the difference between group a and group b is '<a'  and '<span', group c just shows another implementation of jump.
#### Conclusion

1. Test Anchor 7 works in Typora,VsCode and GFM for the use to **jump to a header**.

2. When it comes to **jump to a part which is not a header**,1,3,5 (id) work in VsCode,2,4,6 (name) work in Typora.
3. The <a> tag defines a **hyperlink**,'<span' is used for **mark up a part of a document.**,they are interchangeable here.

* References [Typora docs](https://support.typora.io/Links/#html-a-tag)
#### Here comes the test ,bottom-up is recommended.


# Anchor 1

```html
Anchor1：<a id="anchor1">Anchor1</a>  
Jump1：<a href="#anchor1">Link to Anchor1</a>
```

Anchor1：<a id="anchor1">Anchor1</a>  


# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1

Jump1：<a href="#anchor1">Link to Anchor1</a>

# Anchor 2

```html
Anchor2：<a name= "anchor2">Anchor2</a>
Jump2：<a href="#anchor2">Link to Anchor2</a>
```

Anchor2：<a name= "anchor2">Anchor2</a>


# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1

Jump2：<a href="#anchor2">Link to Anchor2</a>

# Anchor 3

```html
Anchor3：<span id="anchor3">Anchor3</span> 
Jump3：<a href="#anchor3">Link to Anchor3</a>
```

Anchor3：<span id="anchor3">Anchor3</span>  


# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1

Jump3：<a href="#anchor3">Link to Anchor3</a>

# Anchor 4

```html
Anchor4：<span name= "anchor4">Anchor4</span>
Jump4：<a href="#anchor4">Link to Anchor4</a>
```

Anchor4：<span name= "anchor4">Anchor4</span>


# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1

Jump4：<a href="#anchor4">Link to Anchor4</a>

# Anchor 5

```html
Anchor5：<a id="anchor5">Anchor5</a>
Jump5：[Link to Anchor5](#anchor5)
```

Ancho5r：<a id="anchor5">Anchor5</a>


# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1

Jump5：[Link to Anchor5](#anchor5)

# Anchor 6

```html
Anchor6：<a name="anchor6">Anchor6</a>
Jump6：[Link to Anchor6](#anchor6)
```

Anchor6：<a name="anchor6">Anchor6</a>


# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1

Jump6：[Link to Anchor6](#anchor6)

# Anchor7

```html
Anchor7： Header :# Anchor7
Jump7：[Link to Anchor7](#Anchor7)
```


# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1

# 1



Anchor7： Header :# Anchor7
Jump7：[Link to Anchor7](#Anchor7)

