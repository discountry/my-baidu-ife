---
layout: post
title: 任务三：三栏式布局
category: html&css
---

## Lesson

* [任务三：三栏式布局](http://ife.baidu.com/course/detail/id/94)

## References

* [Web 建站技术中，HTML、HTML5、XHTML、CSS、SQL、JavaScript、PHP、ASP.NET、Web Services 是什么？](https://www.zhihu.com/question/22689579)
* [MDN HTML 入门](https://developer.mozilla.org/zh-CN/docs/Web/Guide/HTML/Introduction)
* [SemanticUI Theming Examples](http://semantic-ui.com/examples/theming.html)

## Demo

* [example page](/example)

## Task

* [HTML Tags preview](https://codepen.io/discountry/pen/mWyXQx?editors=1000)
* [HTML Tags source code](https://github.com/discountry/my-baidu-ife/blob/master/codes/html&css/1-html-tags.html)

**html**

```html
<H1>This is h1 title</H1>
<h2>This is h2 title</h2>
<h3>This is h3 title</h3>
<h4>This is h4</h4>
<h5>This is h5</h5>
<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Blanditiis, repellat earum similique sunt, facilis eos, neque vitae aut magnam, eius saepe culpa aliquid iure soluta expedita amet incidunt tempora! Quasi.</p>

<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. At <a href="">perspiciatis</a> eveniet, doloribus odit hic magni <b>excepturi</b> harum nam sint error quos <strong>reprehenderit</strong> tempora! Maxime, quod, consequuntur. <i>Minus eius et aliquid!</i></p>

<p>Lorem <small>ipsum dolor sit amet</small>, consectetur adipisicing elit. Quia, similique. Esse dolor placeat <em>quisquam ut temporibus voluptatum</em>, doloribus expedita, saepe provident architecto iusto beatae obcaecati modi cum excepturi. <abbr title="attribute">Est, esse.</abbr></p>
<!--address-->
<address>
    You can contact author at <a href="http://www.somedomain.com/contact">www.somedomain.com</a>.<br>
    If you see any bugs, please <a href="mailto:webmaster@somedomain.com">contact webmaster</a>.<br>
    You may also want to visit us:<br>
    Mozilla Foundation<br>
    1981 Landings Drive<br>
    Building K<br>
    Mountain View, CA 94043-0801<br>
    USA
  </address>
<!--area-->
<map name="primary">
  <area shape="circle" coords="75,75,75" onclick="alert('left')">
  <area shape="circle" coords="275,75,75" onclick="alert('right')">
</map>
<img usemap="#primary" src="http://placehold.it/350x150" alt="350 x 150 pic">
<!--article-->
<article class="film_review">
  <header>
    <h2>Jurassic Park</h2>
  </header>
  <section class="main_review">
    <p>Dinos were great!</p>
    <aside>
      <p>
        The movie earned $87 million during its initial release.
      </p>
    </aside>
  </section>
  <article class="user_review">
    <p>I agree, dinos are my favorite.</p>
    <footer>
      <p>
        Posted on
        <time datetime="2015-05-17 19:00">May 17</time> by Tom.
      </p>
    </footer>
  </article>
  </section>
  <footer>
    <p>
      Posted on
      <time datetime="2015-05-15 19:00">May 15</time> by Staff.
    </p>
  </footer>
</article>

<!-- Simple audio playback -->
<audio src="http://developer.mozilla.org/@api/deki/files/2926/=AudioTest_(1).ogg" controls="controls">
  Your browser does not support the <code>audio</code> element.
</audio>

<base target="_blank" href="http://www.example.com/page.html">

<p dir="ltr">This arabic word <bdi>ARABIC_PLACEHOLDER</bdi> is automatically displayed right-to-left.</p>

<p>This text will go left to right.</p>
<p><bdo dir="rtl">This text will go right
to left.</bdo></p>

<blockquote cite="http://developer.mozilla.org">
  <p>This is a quotation taken from the Mozilla Developer Center.</p>
</blockquote>

<button name="button">Click me</button>

<br />

<canvas id="canvas" width="300" height="300">
  An alternative text describing what your canvas displays. 
</canvas>

<p>More information can be found in <cite>[ISO-0000]</cite>.</p>

<p>This is how we declare a Javascript variable:
  <br/>
    <code>var i = 0;</code>
</p>

<p>Table with colgroup and col</p>
<table>
  <caption>Awesome caption</caption>
  <colgroup>
    <col style="background-color: #0f0">
    <col span="1">
    <col style="background-color: red">
  </colgroup>
  <tr>
    <th>Lime</th>
    <th>Lemon</th>
    <th>Orange</th>
  </tr>
  <tr>
    <td>Green</td>
    <td>Yellow</td>
    <td>Orange</td>
  </tr>
</table>

<nav>
  <ul>
    <li><a href="">First Link</a></li>
    <li><a href="">Second Link</a></li>
    <li>Third Link</li>
    <li>Fourth Link</li>
  </ul>
</nav>

<p>A common form that includes input tags</p>
<form action="getform.php" method="get">
  <label>First name: <input type="text"></label><br>
  <label>Last name: <input type="text"></label><br>
  <label>E-mail: <input type="email"></label><br>
  <input type="submit" value="Submit">
</form>

<p>Type the following in the Run dialog:
  <kbd>cmd</kbd><br />Then click the OK button.</p>

<!-- Form with fieldset, legend, and label -->
<form action="" method="post">
  <fieldset>
    <legend>Title</legend>
    <input type="radio" id="radio">
    <label for="radio">Click me</label>
  </fieldset>
</form>

<p>你<em>开始</em>学习HTML了.</p>

<article>
  <h3>This is a title.</h3>
</article>

<img src="https://ss0.bdstatic.com/5aV1bjqh_Q23odCf/static/superman/img/logo/bd_logo1_31bdc765.png" alt="" />
```

## Note

* [HTML Character](https://www.w3.org/TR/2011/WD-html5-20110113/named-character-references.html)
* [MDN HTML element reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)

