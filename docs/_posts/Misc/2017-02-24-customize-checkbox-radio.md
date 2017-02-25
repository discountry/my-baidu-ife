---
layout: post
title: 自定义checkbox， radio样式
category: Misc
---

## Lesson

* [自定义checkbox， radio样式](http://ife.baidu.com/course/detail/id/23)

## References

* [Semantic-UI checkbox.css](https://github.com/Semantic-Org/Semantic-UI/blob/master/dist/components/checkbox.css)
* [MDN label](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/label)
* [MDN ::after](https://developer.mozilla.org/en-US/docs/Web/CSS/::after)
* [MDN ::before](https://developer.mozilla.org/en-US/docs/Web/CSS/::before)
* [CSS Selector Reference](https://www.w3schools.com/cssref/css_selectors.asp)

## Task

* [Customized checkbox&radio preview](http://codepen.io/discountry/pen/RpNgmz?editors=1100)
* [Customized checkbox&radio source code](https://github.com/discountry/my-baidu-ife/blob/master/codes/Misc/customized-checkbox&radio.html)


**html**

```html
<h1>Customized inputs</h1>
    <div class="container">
        <h2>Background-image</h2>
        <div class="row1">
            <input type="checkbox" id="checkbox" />
            <label for="checkbox"></label>
            <input type="radio" id="radio" />
            <label for="radio"></label>
        </div>
        <h2>:before :after</h2>
        <div class="row2">
            <div class="box">
                <input type="checkbox" id="checkbox2" />
                <label for="checkbox2"></label>
            </div>
            <div class="box">
                <input type="radio" id="radio2" />
                <label for="radio2"></label>
            </div>
        </div>
    </div>
```

**scss**

```scss
.row1 {
  input[type='checkbox'] {
    display: none;
  }
  input[type='checkbox'] + label {
    background: url('http://p1.bqimg.com/567571/99322cf8c3283e42.png') no-repeat;
    background-position: -24px -32px;
    height: 16px;
    width: 16px;
    display: inline-block;
    cursor: pointer;
  }
  input[type='checkbox']:checked + label {
    background-position: -59px -32px;
  }
  input[type='radio'] {
    display: none;
  }
  input[type='radio'] + label {
    background: url('http://p1.bqimg.com/567571/99322cf8c3283e42.png') no-repeat;
    background-position: -24px -10px;
    height: 16px;
    width: 16px;
    display: inline-block;
    cursor: pointer;
  }
  input[type='radio']:checked + label {
    background-position: -59px -10px;
  }
}

.row2 {
  .box {
    position: relative;
    display: inline-block;
    min-height: 17px;
    font-size: 1rem;
    line-height: 17px;
    min-width: 17px;
  }
  input {
    cursor: pointer;
    position: absolute;
    top: 0;
    left: 0;
    opacity: 0!important;
    z-index: 3;
    width: 16px;
    height: 16px;
  }
  label:before {
    position: absolute;
    top: 0;
    left: 0;
    width: 16px;
    height: 16px;
    content: '';
    border: 1px solid #9e9e9e;
  }
  input[type=radio]~label:before {
    border-radius: 500rem;
  }
  input[type=radio]:checked~label:after {
    content: '●';
    font-size: 16px;
    line-height: 15px;
    width: 18px;
  }
  input[type=checkbox]:checked~label:after {
    content: '\2714';
  }
  input:checked~label:after {
    position: absolute;
    font-size: 14px;
    top: 0;
    left: 0;
    width: 17px;
    height: 17px;
    text-align: center;
    color: #d73d32;
  }
  input:checked~label:before {
    border-color:#d73d32;
  }
}

.container {
  height: 20rem;
}

.row1,
.row2 {
  width: 100%;
  align-items: center;
  justify-content: center;
  display: flex;
}

label {
  margin: 1rem;
}

h1,
h2 {
  text-align: center;
  width: 100%;
}
```

## Note

**获取雪碧图内容坐标**

![ps sprite](https://ooo.0o0.ooo/2017/02/25/58b16c5721ecc.png)


**CSS特殊字符**

* [Character Entities](https://brajeshwar.github.io/entities/)

**CSS特殊选择器**

```css
div + p {
    /*  Selects all <p> elements that are placed immediately after <div> elements
     * CSS2中 选择紧接在div后面的p
    */
}

div ~ p {
    /*  Selects every <ul> element that are preceded by a <p> element
     *  CSS3中 选择前面跟着div的p
    */
}
```
