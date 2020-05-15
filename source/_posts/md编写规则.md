---
title: md编写规则
date: 2020-05-15 11:26:42
tags: markdown
categories: Init
mathjax: true
---

    # 标题H1
# 标题H1
    ## 标题H2
## 标题H2
    ### 标题H3
### 标题H3
    #### 标题H4
#### 标题H4
    ##### 标题H5
##### 标题H5
    ###### 标题H5
###### 标题H5

### 字符效果和横线等
    ---- 横线
----
    ~~删除线~~
~~删除线~~ <s>删除线（开启识别HTML标签时）</s>

    *斜体字*   或  _斜体字_
*斜体字*      _斜体字_

    **粗体**  __粗体__
**粗体**  __粗体__
    
    ***粗斜体*** ___粗斜体___
***粗斜体*** ___粗斜体___
    
    上标：X<sup>2</sup>，下标：O<sub>2</sub>
上标：X<sup>2</sup>，下标：O<sub>2</sub>

**缩写(同HTML的abbr标签)**
> 即更长的单词或短语的缩写形式，前提是开启识别HTML标签时，已默认开启

    <abbr title="Hyper Text Markup Language">HTML</abbr>
<abbr title="Hyper Text Markup Language">HTML</abbr>

### 引用 Blockquotes
    > 引用文本 Blockquotes
> 引用文本 Blockquotes
> 
> 引用：如果想要插入空白换行`即<br />标签`，在插入处先键入两个以上的空格然后回车即可

### 锚点与链接 Links
    [普通链接](https://www.mdeditor.com/)
[普通链接](https://www.mdeditor.com/)

    [普通链接带标题](https://www.mdeditor.com/ "普通链接带标题")
[普通链接带标题](https://www.mdeditor.com/ "普通链接带标题")

    直接链接：<https://www.mdeditor.com>
直接链接：<https://www.mdeditor.com>

~~[锚点链接][anchor-id]~~
~~[anchor-id]: https://www.mdeditor.com/~~

    邮箱地址自动链接 test.test@gmail.com  www@vip.qq.com
test.test@gmail.com    www@vip.qq.com

    github自动链接 @pandao （hexo不适用）
~~@pandao~~

### 多语言代码高亮 Codes

#### 行内代码 Inline code

    执行命令：`npm install marked`
执行命令：`npm install marked`

#### 缩进风格

即缩进四个空格，也做为实现类似 `<pre>` 预格式化文本 ( Preformatted Text ) 的功能。

    <?php
        echo "Hello world!";
    ?>
预格式化文本：

    | First Header  | Second Header |
    | ------------- | ------------- |
    | Content Cell  | Content Cell  |
    | Content Cell  | Content Cell  |

#### JS代码

    (```javascript) 注：实际使用无括号
    function test() {
    console.log("Hello world!");
    }
    (```)

```javascript
function test() {
	console.log("Hello world!");
}
```

#### HTML 代码 HTML codes

    (```html) 注：实际使用无括号
    <html></html>
    (```)

```html
<!DOCTYPE html>
<html>
    <head>
        <mate charest="utf-8" />
        <meta name="keywords" content="Editor.md, Markdown, Editor" />
        <title>Hello world!</title>
        <style type="text/css">
            body{font-size:14px;color:#444;font-family: "Microsoft Yahei", Tahoma, "Hiragino Sans GB", Arial;background:#fff;}
            ul{list-style: none;}
            img{border:none;vertical-align: middle;}
        </style>
    </head>
    <body>
        <h1 class="text-xxl">Hello world!</h1>
        <p class="text-green">Plain text</p>
    </body>
</html>
```
### 图片 Images

图片加链接 (Image + Link)：

    [![](/images/404.jpg)](/images/404.jpg "404")
[![](/images/404.jpg)](/images/404.jpg "404")

----
### 列表 Lists

#### 无序列表（减号）Unordered Lists (-)

`- 列表一`
- 列表一

#### 无序列表（星号）Unordered Lists (*)

`* 列表一`
* 列表一

#### 无序列表（加号和嵌套）Unordered Lists (+)

    + 列表一
    + 列表二
        + 列表二-1
    + 列表三
        * 列表三-1

+ 列表一
+ 列表二
    + 列表二-1
+ 列表三
    * 列表三-1

#### 有序列表 Ordered Lists (-)

    1. 第一行
    2. 第二行

1. 第一行
2. 第二行

#### GFM task list

    - [x] GFM task list 1
    - [ ] GFM task list 2
        - [x] GFM task list 2-1
    - [ ] GFM task list 3
        - [ ] GFM task list 3-1

- [x] GFM task list 1
- [ ] GFM task list 2
    - [x] GFM task list 2-1
- [ ] GFM task list 3
    - [ ] GFM task list 3-1

----

### 绘制表格 Tables

    注：分割线有无‘:’都可，效果一样
    | 项目        | 价格    |  数量   |
    | --------   | -----:  | :----:  |
    | 计算机      | $1600   |   5    |
    | 手机        |   $12   |   12   |
    | 管线        |    $1   |  234   |

| 项目        | 价格    |  数量   |
| --------   | -----:  | :----:  |
| 计算机      | $1600   |   5    |
| 手机        |   $12   |   12   |
| 管线        |    $1   |  234   |

----

#### 特殊符号 HTML Entities Codes

    &copy; &  &uml; &trade; &iexcl; &pound;
&copy; &  &uml; &trade; &iexcl; &pound;

    &amp; &lt; &gt; &yen; &euro; &reg; &plusmn; &para; &sect; &brvbar; &macr; &laquo; &middot;
&amp; &lt; &gt; &yen; &euro; &reg; &plusmn; &para; &sect; &brvbar; &macr; &laquo; &middot;

    X&sup2; Y&sup3; &frac34; &frac14;  &times;  &divide;   &raquo;
X&sup2; Y&sup3; &frac34; &frac14;  &times;  &divide;   &raquo;

    18&ordm;C  &quot;  &apos;
18&ordm;C  &quot;  &apos;

### Emoji表情 :smiley:
    
    暂不支持

#### 反斜杠 Escape

    这里只是展示反斜杠的作用：\*literal asterisks\*
\*literal asterisks\*

### 科学公式 TeX(KaTeX)

    $$E=mc^2$$
$$E=mc^2$$

    行内的公式$$E=mc^2$$行内的公式，行内的$$E=mc^2$$公式。
行内的公式$$E=mc^2$$行内的公式，行内的$$E=mc^2$$公式。

    $$x > y$$
$$x > y$$

    $$(\sqrt{3x-1}+(1+x)^2)$$
$$(\sqrt{3x-1}+(1+x)^2)$$

    $$\sin(\alpha)^{\theta}=\sum_{i=0}^{n}(x^i + \cos(f))$$
$$\sin(\alpha)^{\theta}=\sum_{i=0}^{n}(x^i + \cos(f))$$

多行公式：

    $$
    \displaystyle
    \left( \sum\_{k=1}^n a\_k b\_k \right)^2
    \leq
    \left( \sum\_{k=1}^n a\_k^2 \right)
    \left( \sum\_{k=1}^n b\_k^2 \right)
    $$

$$
\displaystyle
\left( \sum\_{k=1}^n a\_k b\_k \right)^2
\leq
\left( \sum\_{k=1}^n a\_k^2 \right)
\left( \sum\_{k=1}^n b\_k^2 \right)
$$

    $$
    \displaystyle
        \frac{1}{
            \Bigl(\sqrt{\phi \sqrt{5}}-\phi\Bigr) e^{
            \frac25 \pi}} = 1+\frac{e^{-2\pi}} {1+\frac{e^{-4\pi}} {
            1+\frac{e^{-6\pi}}
            {1+\frac{e^{-8\pi}}
             {1+\cdots} }
            }
        }
    $$

$$
\displaystyle
    \frac{1}{
        \Bigl(\sqrt{\phi \sqrt{5}}-\phi\Bigr) e^{
        \frac25 \pi}} = 1+\frac{e^{-2\pi}} {1+\frac{e^{-4\pi}} {
        1+\frac{e^{-6\pi}}
        {1+\frac{e^{-8\pi}}
         {1+\cdots} }
        }
    }
$$

    $$
    f(x) = \int_{-\infty}^\infty
        \hat f(\xi)\,e^{2 \pi i \xi x}
        \,d\xi
    $$

$$
f(x) = \int_{-\infty}^\infty
    \hat f(\xi)\,e^{2 \pi i \xi x}
    \,d\xi
$$

### 绘制流程图 Flowchart

    (```)flow
    st=>start: 用户登陆
    op=>operation: 登陆操作
    cond=>condition: 登陆成功 Yes or No?
    e=>end: 进入后台
    st->op->cond
    cond(yes)->e
    cond(no)->op
    (```)

```flow
st=>start: 用户登陆
op=>operation: 登陆操作
cond=>condition: 登陆成功 Yes or No?
e=>end: 进入后台

st->op->cond
cond(yes)->e
cond(no)->op
```

### 绘制序列图 Sequence Diagram

    (```)sequence
    Alice->Bob: Hello Bob, how are you?
    Note right of Bob: Bob thinks
    Bob-->Alice: I am good thanks!
    (```)

```sequence
Alice->Bob: Hello Bob, how are you?
Note right of Bob: Bob thinks
Bob-->Alice: I am good thanks!
```

### End