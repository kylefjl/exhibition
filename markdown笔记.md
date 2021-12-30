<center><font size=8 famil='黑体'>Markdown笔记</font>


***********

[Toc]

# Markdown简介

Markdown是一种轻量级标记语言，创始人为John Gruber。
Markdown是为了更简单方便地书写 HTML ，使我们更加专注于内容写作本身。

[Typora Support](https://support.typora.io/)

善于运用官方文档，可以解决许多问题

# 正文

## 标题格式类

|   名称   |                     md标记                      |   md例子    |
| :------: | :---------------------------------------------: | :---------: |
|   标题   |                      `###`                      |    如上     |
|  分割线  |                   `*********`                   |    如上     |
|   目录   |                     `[TOC]`                     |    如上     |
| 强制分页 | `<div STYLE="page-break-after: always;"></div>` | 在pdf中可见 |

## 文本类

| 名称 | md标记 | md例子     |
| :------------: | :-------------: | :------------: |
| 加粗 |`**文字**` | **这是粗体** |
| 斜体 | `_文字_` `*文字*` | *斜体*   _斜体_ |
| 删除线 | `~~文字~~` | ~~删除~~ |
| 高亮 | `==文字==` | ==高亮== |
| 换行 | `<br /> 或 <br/> 或 <br/>或shift加enter` | 你好<br/>世界 <br/> |
| 居中 | `<center>` | 如下 |
| 字体字号 | `<font size=2 famil='黑体'>点击显示 </font>` | <font size=4 famil='黑体'>markdown笔记</font> |

<center><font size=4 famil='黑体'>markdown笔记</font>

## 引用类

| 名称 | md标记 | md例子 |
| :--: | :----: | :----: |
| 引用 | `>` | 如下 |
| 嵌套引用 | `>>` | 如下 |
| 链接 | `[kyle的 github] ` `(https://github.com/kylefjl)` | [kyle的 github](https://github.com/kylefjl) |
| 邮箱 | <  > | <l-------@gmail.com> |
| 脚注 | `脚注[^1] ` ` [1]:http://baidu.com` | 脚注[^1] |
| emoji | `:sparkles:`， 查询[网站](https://www.webfx.com/tools/emoji-cheat-sheet) | :+1: :sparkles: :camel: :tada: |

引用定理

> 罗尔定理
>
> > 罗尔定理
> >
> > :+1: :sparkles: :camel: :tada: 
> >
> > :rocket: :metal: :heart_eyes: :sob:

[^1]:http://baidu.com

## 列表表格类

|   名称   |                md标记                | md格式 |
| :------: | :----------------------------------: | :----: |
| 无序标记 |   `-` 或`*` 或 `+` ，加tab为下一级   |  如下  |
| 有序列表 |              `1. ` 2.`               |  如下  |
|   表格   |         \|名称\|标记\|格式\|         | 如该表 |
|   代办   | `- [x]`  已 完 成    `- [ ]`  未完成 |  如下  |
|  流程图  |              ````flow`               |  如下  |

* 无序列表
  - 一
  - 二

- 有序列表
  1. 第一条
  2. 第二条
- 代办
  - [x] 代办1
  - [ ] 代办2 

- 流程图

  ````flow
  ```flow
  st=>start: Start
  op=>operation: Your Operation
  cond=>condition: Yes or No?
  e=>end
  st->op->cond
  cond(no)->op
  cond(yes)->e
  cond(no)->op
  ````
  


## 代码类

|    名称    |    md标记     |      md例子      |
| :--------: | :-----------: | :--------------: |
| 代码块高亮 | ` ```python ` |       如下       |
|  行内代码  |     ``` `     | `print("hello")` |

~~~python
python 块
string = 'Python'
print(string)
~~~

## 图片类

|   名称   |                           md标记                            |                            md例子                            |
| :------: | :---------------------------------------------------------: | :----------------------------------------------------------: |
|   图片   |                          截图插入                           | ![image-20211230184019744](https://raw.githubusercontent.com/kylefjl/clouding/main/img/202112302306305.png) |
| 图片上传 |             格式->图像->全部上传（github图床）              | <img src="https://raw.githubusercontent.com/kylefjl/clouding/main/img/202112301841628.png" alt="image-20211230184019744" style="zoom:100%;" /> |
| 图片大小 | 先右键缩小再自己调整 style="width:10%;"   style="zoom:10%;" | <img src="https://raw.githubusercontent.com/kylefjl/clouding/main/img/202112301841628.png" alt="image-20211230184019744" title=" 图片文本" style="zoom:150%;" /> |
| 悬停文本 |                      title="图片文本"                       | <img src="https://raw.githubusercontent.com/kylefjl/clouding/main/img/202112301841628.png" alt="image-20211230184019744" title=" 图片文本" style="zoom:150%;" /> |
|   对齐   |               align="left"   align对齐的意思                |                             如下                             |

对齐方式

<img src="https://raw.githubusercontent.com/kylefjl/clouding/main/img/202112301841628.png" alt="image-20211230184019744" title="图片文本" align="left" /><img src="https://raw.githubusercontent.com/kylefjl/clouding/main/img/202112302306307.png" alt="image-20211230193713080" style="zoom:80%;" align="right" />



<img src="https://raw.githubusercontent.com/kylefjl/clouding/main/img/202112302306308.png" alt="image-20211230193549339"  title="图片文本" style="zoom:80%;"  align="mid" />

## 数学公式

|    名称    |     md标记      |                 md例子                  |
| :--------: | :-------------: | :-------------------------------------: |
|  行内公式  |  `$`公式`  $ `  | 行 内 公 式 $\sqrt{x^2+y^2}$ 行 内 公式 |
| 单独行显示 | `$$`  公式 `$$` |                  如下                   |
|    标号    |    `\tag{a}`    |                  如下                   |

$$
f(x) = \sum_{i=0}^{N} \int_{a}^{b} g(t,i) \text{d}t \tag{a}
$$



### 附1.上下标，无穷，矢量，累加累乘，极限

|            LaTex代码            |            数学表达式             |
| :-----------------------------: | :-------------------------------: |
|               x^2               |               $x^2$               |
|               y_1               |               $y_1$               |
|             \infty              |             $\infty$              |
|             \vec{F}             |             $\vec{F}$             |
|       \sum_{i=1}^{n}{a_i}       |       $\sum_{i=1}^{n}{a_i}$       |
|      \prod_{i=1}^{n}{a_i}       |      $\prod_{i=1}^{n}{a_i}$       |
| \lim_{a\rightarrow+\infty}{a+b} | $\lim_{a\rightarrow+\infty}{a+b}$ |

### 附2.加减乘，分式，根号，省略号,大于等于，小于等于

|            LaTex代码             |              数学表达式              |
| :------------------------------: | :----------------------------------: |
|             a+b-c*d              |              $a+b-c*d$               |
|             a\div{b}             |              $a\div{b}$              |
|             a\pm{b}              |              $a\pm{b}$               |
|           \frac{a}{b}            |            $\frac{a}{b}$             |
|             \sqrt{b}             |              $\sqrt{b}$              |
| \cdots  <br />\vdots<br />\ddots | $\cdots$<br />$\vdots$<br />$\ddots$ |
|               \leq               |                $\leq$                |
|               \geq               |                $\geq$                |

### 附3.三角函数

|  LaTex代码   |   数学表达式   |
| :----------: | :------------: |
| \sin(\theta) | $\sin(\theta)$ |
| \cos(\theta) | $\cos(\theta)$ |
| \tan(\theta) | $\tan(\theta)$ |
| \cot(\theta) | $\cot(\theta)$ |

### 附4. 希腊字母

|  LaTex代码  |  数学表达式   |
| :---------: | :-----------: |
|   \alpha    |   $\alpha$    |
|    \beta    |    $\beta$    |
|   \gamma    |   $\gamma$    |
|   \delta    |   $\delta$    |
|  \epsilon   |  $\epsilon$   |
| \varepsilon | $\varepsilon$ |
|    \eta     |    $\eta$     |
|   \theta    |   $\theta$    |
|   \kappa    |   $\kappa$    |
|    \iota    |    $\iota$    |
|    \zeta    |    $\zeta$    |
|   \lambda   |   $\lambda$   |
|     \mu     |     $\mu$     |
|    \phi     |    $\phi$     |
|     \pi     |     $\pi$     |
|    \rho     |    $\rho$     |
|     \xi     |     $\xi$     |
|     \mu     |     $\mu$     |
|  \upsilon   |  $\upsilon$   |
|   \varphi   |   $\varphi$   |
|    \chi     |    $\chi$     |
|    \psi     |    $\psi$     |
|   \omega    |   $\omega$    |

## 矩阵

|     名称     |                            md标记                            |                            md例子                            |
| :----------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
|   简单矩阵   | 使用`\begin{matrix}…\end{matrix}`生成， 每一行以`\\`结尾表示换行，元素间以`&`间隔，式子的表示序号`\tag{1}`（右边的序号） | $\begin{matrix} 1 & 2 & 3 \\ 4 & 5 & 6 \\ 7 & 8 & 9 \end{matrix} \tag{1}$ |
| 左右括号矩阵 | \left\{   加        \right\}  <br />\left[   加     \right] <br />\left(   加     \right） | $\left\{\begin{matrix} 1 & 2 & 3 \\ 4 & 5 & 6 \\ 7 & 8 & 9 \end{matrix} \tag{1} \right\} $ |
|    行列式    | 使用`\begin{vmatvrix}…\end{vmatrix}`生成， 每一行以`\\`结尾表示换行，元素间以`&`间隔，式子的表示序号`\tag{1}`（右边的序号） | $\begin{vmatrix}   1 & 2 & 3 \\  4 & 5 & 6 \\   7 & 8 & 9 \end{vmatrix}$ |

csdn与typoramarkdown规则不同，用图片展示

![image-20211230232747887](https://raw.githubusercontent.com/kylefjl/clouding/main/img/202112302328444.png)

## 参考链接：[知乎]([Typora数学公式汇总（Markdown） - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/261750408))

