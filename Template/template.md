---
title: Keynote
separator: ---
verticalSeparator: -v-
# Themes: beige/black/blood/league/moon/night/serif/simple/sky/solarized/white
theme: white 
# Transitions: 'concave/convex/cube/fade/none/page/slide/zoom'
revealOptions:
    transition: slide
---

<!-- .slide: data-transition="zoom" -->
## Title of the Keynote

<div style="margin-bottom:2cm;"></div>

<div style="font-size:30pt; padding-bottom:1.5cm">organization</div>

<div style="font-size:25pt;">Your Name</div>

<div style="font-size:20pt; padding-top:1.5cm">date</div>

Note: put speaker notes for this slide here.

---

## About this template

<div class="content">

- [Markdown source code of this template](https://github.com/howardhsumail/revealJS-Tutorial/blob/main/Template/template.md?plain=1)
- [revealJS-Tutorial Github Repository](https://github.com/howardhsumail/revealJS-Tutorial.git)
- [Economics Presentation Example](https://www.haochehsu.com/slides/revealJS/index.html)
- Please [contact](mailto:howardhsumail@gmail.com) the [author](https://www.haochehsu.com/) for help, comments, error reporting.

</div>

Note: put speaker notes for this slide here.

---

<!-- .slide: data-transition="slide" -->
# Single line title 

<span style="font-size: 30px">continue from here, you can go RIGHT ($\rightarrow$) or DOWN ($\downarrow$)</span>

-v-

### Vertical Page Subtitle

<div class="content">

Aenean quam felis, tristique vel iaculis sollicitudin, iaculis nec sem. Nulla venenatis sem lorem, at mollis nulla semper vel. Morbi.

</div>

Note: put speaker notes for this slide here.

---

<!-- .slide: data-transition="convex" -->
## Unordered List

<div class="content">

- Item 1
- Phasellus imperdiet quam ultricies, scelerisque sem lacinia, egestas libero. Praesent.
  - Item 2a
    - Item 2ai

</div>

Note: put speaker notes for this slide here.

---

<!-- .slide: data-transition="convex" -->
## Ordered List

<div class="content">

1. Item 1
2. Item 2
    - Item 2a
3. Morbi gravida, ligula non gravida sodales.
    - Item 3a
      - Item 3ai

</div>

Note: put speaker notes for this slide here.

---

# Fragment
<span style="font-size: 30px">DOWN ($\downarrow$) for more</span>

-v-

### The following items <div style="margin-bottom:-0.7cm;"></div>
### will appear in customized order

<div class="content">

- <!-- .element: class="fragment" data-fragment-index="1" --> This item appears <b>first</b>. 
  - <!-- .element: class="fragment" data-fragment-index="1" --> Vivamus sollicitudin purus eget lobortis porttitor. 
- <!-- .element: class="fragment" data-fragment-index="3" --> This item appears <b>third</b>.
- <!-- .element: class="fragment" data-fragment-index="2" -->This item appears <b>second</b>.

</div>

-v-

### Fragment animation

<div class="content">

<p class="fragment">Fade in</p>
<p class="fragment fade-out">Fade out</p>
<p class="fragment highlight-green">Highlight green</p>
<p class="fragment fade-in-then-out">Fade in, then out</p>
<p class="fragment highlight-current-red">Highlight red, then back to original</p>
<p class="fragment fade-up">Slide up while fading in</p>
<p class="fragment grow">Growing text</p>

*** 
<br>

Fragment Effects: [LINK](https://revealjs.com/fragments/)

</div>

---

<!-- .slide: data-transition="zoom" -->
# Formatting
<span style="font-size: 30px">DOWN ($\downarrow$) for more</span>

-v-

## Text format

<div class="content">

<div style="display: flex;">
<div style="flex: 50%;">

**Bold** text or <b>Bold</b>

*Italic* text or <em>Italic</em>

<u>underline</u> text

<del>strikethrough</del> text

***Bold and Italic*** text

<mark>marked</mark> text

>Blockquotes text

</div>
<div style="flex: 50%;">

<span style="color: #23B034">Customized color</span> text

text <sup>SUPscript</sup>

text <sub>SUBscript</sub>

<span style="font-size: 50px">Customized size</span> text

<!-- Arial/Verdana/Helvetica/Tahoma/Trebuchet MS/Times New Roman/Georgia/Garamond/Courier New/Brush Script MT -->
<span style="font-family:Brush Script MT;">Customized font</span> text

</div>
</div>

</div>

-v-

## Alignment

<div class="content">

<div style="text-align: left;">

The following text is **aligned left**. Duis in tempor nisi, eget lobortis velit. Nunc consequat, urna.

</div>

<div style="text-align: right;">

The following text is **aligned right**. Duis in tempor nisi, eget lobortis velit. Nunc consequat, urna.

</div>

<div style="text-align: justify;">

The following text is **aligned justify**. Duis in tempor nisi, eget lobortis velit. Nunc consequat, urna.

</div>

<div style="text-align: center;">

The following text is **aligned center**. Duis in tempor nisi, eget lobortis velit. Nunc consequat, urna.

</div>

</div>

-v-

## Spacing

<div class="content">

Use `&nbsp;` to add &nbsp; &nbsp; &nbsp; **horizontal** spacing.

***

Use `***` to add **separator**.

***

Use `<br>` to add </br></br> **vertical** spacing.

<div style="margin-bottom:4cm;"></div>

or with HTML `<div style="margin-bottom:4cm;"></div>`.

</div>

---

<!-- .slide: data-transition="concave" -->
## Hyperlink

- External link: [www.haochehsu.com](https:www.haochehsu.com)

- Internal link: | [Internal 1](#/7/1) &nbsp; | &nbsp; [Internal 2](#/7/2) |

-v-

### Hyperlink internal slides 1

<div class="content">

In eu dictum ipsum, in congue ligula. In lacinia nulla odio, vel mollis ante cursus eu. Integer quis risus sit amet magna tincidunt convallis. Suspendisse dolor est, egestas id semper.

<div style="margin-bottom:3.5cm;"></div>

<span style="font-size: 30px">[Go back](#/7)</span>

</div>

-v-

### Hyperlink internal slides 2

<div class="content">

Sed eu nunc sed dolor fermentum efficitur et eu nisl. Nulla lacinia arcu nisi, eget faucibus lorem eleifend luctus. Proin posuere auctor cursus. Maecenas viverra condimentum orci non finibus. Fusce.

<div style="margin-bottom:3.5cm;"></div>

<span style="font-size: 30px">[Go back](#/7)</span>

</div>

---

<!-- .slide: data-transition="page" -->
## Math

<div style="font-size:23pt">

Given $y$, $x$, $\Delta$, $\nu$, $\eta$, with the following matrices

<div style="font-size:23pt">
$$\mathcal{L}=\begin{pmatrix}
1 & 2 & 3 & 4 & 5 \\
3 & 4 & 5 & 6 & 7
\end{pmatrix} \text{and} \prod=\begin{vmatrix}
A &B  &C \\
D&  E& F
\end{vmatrix}$$
</div>

<div style="text-align:left;padding-left:2.5cm">Math alignment:</div>

<div style="font-size:23pt">
$$\begin{align}
  y&=\underset{\pi}{\mathbb{E}}\Big(\beta x + \epsilon\Big)\neq\sum\limits_{i}\beta_i(\underbrace{\alpha+\xi}_{\text{variables}}) + \epsilon\\
  &\Longrightarrow \int_{0}^{10}r \left( \dfrac{r}{50} \right)dr\xrightarrow{\text{text here}}\dfrac{r^{3}}{150}\biggr\rvert^{10}_{0}, \forall x\in (a,b)
\end{align}$$
</div>

So from $\widehat{ABCD}$, $\widetilde{ABCD}$, $\widehat{ABCD}$, $\overrightarrow{ABCD}$, and $\overline{ABCD}$, we get the desire $\underline{\text{result}}$.
  
</div>

---

## Code

<div class="content">

<br>

#### Inline code

`mylist = list(filter(lambda x: 'words' not in x, mylist))`

***

<br>

#### Block code

```python
# Long short-term memory (LSTM)
def __init__(self, input_size=1, hidden_size=256, output_size=1):
        super().__init__()
        self.hidden_size = hidden_size
        self.lstm = nn.LSTM(input_size, hidden_size)

        # fully-connected
        self.linear = nn.Linear(hidden_size, output_size)

        self.hidden = (
            torch.zeros(1, 1, self.hidden_size),
            torch.zeros(1, 1, self.hidden_size)
        )
```

</div>

---

## Image

<span class="fragment fade-in-then-out" >
  <img style="width: 70%; border-radius: 5px; box-shadow: 0px 0px 30px 3px #888888;" src="https://www.haochehsu.com/other/volcano.jpg" />
</span>

---

<!-- .slide: data-transition="convex" -->
## Table

<div class="content">

HTML table generator: [LINK](https://www.tablesgenerator.com/html_tables)
<br><br>

<table class="w3-striped">
<thead>
  <tr>
    <th>First Header</th>
    <th>Second Header</th>
    <th>Third Header</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Content from cell 1</td>
    <td>Content from cell 2</td>
    <td>Content from cell 3</td>
  </tr>
  <tr>
    <td>first column</td>
    <td>second column</td>
    <td>third column</td>
  </tr>
  <tr>
    <td>(4,1)</td>
    <td>(4,2)</td>
    <td>(4,3)</td>
  </tr>
  <tr>
    <td>(5,1)</td>
    <td>(5,2)</td>
    <td>(5,3)</td>
  </tr>
</tbody>
</table>

</div>

---

## Video

<iframe width="840" height="560"
src="https://www.youtube.com/embed/pKO9UjSeLew?autoplay=0&mute=1">
</iframe>

<span style="font-size: 20px">Source: <span style="font-style: italic">If Programming Was An Anime</span> ([Joma Tech](https://www.youtube.com/c/JomaOppa))</span>

---

<!-- .slide: data-transition="zoom" -->
<!-- .slide: data-background="#244A7C" -->
## Change Background Color

---

## Keyboard Shortcuts

<div class="content">

- <span style="color: blue">`Shift` + `?`</span>: Look up keyboard shortcuts
- <span style="color: blue">`s`</span>: Open speaker notes view (placed on second screen during presentation)
- <span style="color: blue">`Shift` + $\leftarrow$</span>: Go to first slide
- <span style="color: blue">`Shift` + $\rightarrow$</span>: Go to last slide
- <span style="color: blue">`ESC`</span>: Overview slides
- <span style="color: blue">`F`</span>: Fullscreen
- <span style="color: blue">`B`</span>: Pause (blackout)

</div>

<!-- CSS -->
<style>
.content {
  font-size:26pt !important; 
  line-height:42pt !important;
}
</style>
<base target="_blank"/>
<link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css">
<script src="plugin/math/math.js"></script>
<script>
  Reveal.initialize({ plugins: [ RevealMath.KaTeX ] });
</script>