---
layout: post
title: 任务四：定位和居中问题
category: html&css
---

## Lesson

* [任务四：定位和居中问题](http://ife.baidu.com/course/detail/id/95)

## References

* [HTML和CSS高级指南之二——定位详解](http://www.w3cplus.com/css/advanced-html-css-lesson2-detailed-css-positioning.html)
* [Centering in CSS: A Complete Guide](https://css-tricks.com/centering-css-complete-guide/)
* [Get HTML & CSS Tips In Your Inbox](http://howtocenterincss.com/)

## Task

* [Center position preview](http://codepen.io/discountry/pen/wJBOJb?editors=1100)
* [Center position source code](https://github.com/discountry/my-baidu-ife/blob/master/codes/html&css/4-center-position.html)

**html**

```html
<main>
  <div>
    <div class="top-left circle"></div>
    <div class="block"></div>
    <div class="bottom-right circle"></div>
  </div>
</main>
```

**css**

```css
html,
body {
  height: 100%;
  padding: 0;
  margin: 0;
}

main {
  height: 100%;
  margin: 0 auto;
  display: flex;
  justify-content: center;
  align-items: center;
}

main div {
  background: #ccc;
  color: white;
  width: 400px;
  height: 200px;
  overflow: hidden;
}

.top-left {
  margin: -50px 0 0 -50px;
}

.bottom-right {
  float: right;
  margin: 0 -50px -50px 0;
}

.block {
  width: 100%;
  height: 100px;
}

.circle {
  background-color: #FC0;
  width: 100px;
  height: 100px;
  border: #FC0 1px solid;
  border-radius: 500rem;
}
```

## Note

**如何使 `height: 100%` 生效**

目标的父元素必须指定准确高度，或者其所有父元素高度均为 `100%` 。

```css
html,
body {
  height: 100%;
}

div {
  height: 100%;
}
```

**重置浏览器默认边距**

```css
html,
body {
  padding: 0;
  margin: 0;
}
```

** `margin` 一类描述容器四边的属性的顺序是上右下左**

```css
div {
  margin: -50px 0 0 -50px;
}
```