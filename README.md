# Reveal.js Tutorial

This is a tutorial on utilizing the [reveal.js framework](https://revealjs.com/) with [markdown](https://www.markdownguide.org/) by using the [reveal-md](https://github.com/webpro/reveal-md) tool. Comparing to [Beamer](https://www.overleaf.com/learn/latex/Beamer) which creates PDF slides with `TeX`, `reveal.js` creates browser-based slides (convertible to PDF) with Javascript + HTML + CSS. A comparison between the two tools is [here](https://www.maths.dur.ac.uk/users/s.m.fearn/blog/2020/revealjs/). The workflow can be summarized: Edit the slides in markdown → convert to HTML slides.

🚀 The template can be viewd [here](https://www.haochehsu.com/slides/template/index.html). The tempalte markdown file is [here](https://github.com/howardhsumail/revealJS-Tutorial/blob/main/Template/template.md?plain=1)).

🚀 An presentation example is demonstrated [here](https://www.haochehsu.com/slides/revealJS/index.html). Its markdown file is [here](https://github.com/howardhsumail/revealJS-Tutorial/blob/main/Example/example.md?plain=1).

### Installation

1. Install Node Version Manager (`nvm`)

```shell
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.37.2/install.sh | bash
```

2. Loads `nvm`

```shell
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"
```

3. Install NodeJS

```shell
nvm install v15
```

4. Install `reveal-md`

```shell
npm install -g reveal-md
```

### Usage

- Make HTML slides

```shell
reveal-md yourSlides.md --static outputFolderName
```

Drag the markdown (`.md`) file into the Terminal to obtain the file path. To convert the markdown template to HTML slides, [download](https://github.com/howardhsumail/revealJS-Tutorial/archive/refs/heads/main.zip) and unzip the repository. Then direct the workspace to the `Template` sub-folder: `cd <path to Template folder>`. The the slides (`index.html` in the `Output` folder) can be obtained by `reveal-md template.md --static output`.

- Live view the slides

```shell
reveal-md yourSlides.md -w
```

The terminal will return the following message: `Reveal-server started at http://localhost:xxxx`. If the browser does not pop up, paste `http://localhost:xxxx` into the browser to start live editing.

### Controls

To control the presentation, press `Shift` + `?` to see the keyboard shortcuts. This includes Speaker notes view (`S`), First slide (`Shift` + `←`), Last slide (`Shift` + `→`), Overview (`ESC`), Fullscreen (`F`), and Pause (`B`).

---

### Markdown

Most of the time, we need to rely on HTML + CSS code to control the style and the animation of the slides, so [VS Code](https://code.visualstudio.com/) is the recommended editor. For plain markdown files, [Typora](https://typora.io/) is recommended.

### Slides

In your working directory, there are 2 files: `markdownSlides.md` and `reveal.json`.

#### 1. `reveal.json`

This is the configuration file. You can specify the `margin`, 4 different page indicators (more [options](https://revealjs.com/slide-numbers/)), toggle the visibility of the controller and the bottom progress bar, the `width`, and the `height`.

#### 2. `markdownSlides.md`

Slides are written in markdown ([syntax](https://www.markdownguide.org/basic-syntax/)) with HTML ([syntax](https://www.w3schools.com/html/html5_syntax.asp)) formatting. At the top, you can define the `Title` of the HTML page, background theme (more [options](https://revealjs.com/themes/)), global slide transitions (more [options](https://revealjs.com/transitions/)), horizontal slides separator (`---`), and vertical slides separator (`-v-`). To add speaker view notes, use `Note:` in each slide. For syntax[^1], please refer to the [example](https://github.com/howardhsumail/revealJS-Tutorial/blob/main/Example/example.md?plain=1).

---

###  Design

In this section, we will go through some common designs. 

#### Fragment

Control each element separately (e.g. display list items sequentially). The declaration is added to the end of each element with `x` being the order:

```md
<!-- .element: class="fragment data-fragment-index="x" -->
```

Animation can be added to the element by using the following comment:

```md
<!-- .element: class="fragment animationName" -->
```
The `animationName` can be replaced by one of the 17 [effects](https://revealjs.com/fragments/).

#### Transition

The transition between slides in controlled by the following comment:

```md
<!-- .slide: data-transition="transitionName" -->
```
The `transitionName` can be replaced by the 6 different [effects](https://revealjs.com/transitions/).

#### Adding vertical spaces

```html
<div style="margin-bottom:1cm;"></div>
```

#### Content alignment

```html
<div style="text-align: left;">
 The contents here including text, images,... will align to left.
</div>
```
More alignment properties can be found [here](https://www.w3schools.com/cssref/pr_text_text-align.ASP).

#### Padding

To re-position, for example, a left-aligned paragraph, we can add paddings:

```html
<div style="padding-left:5cm;">
 Something or another <div></div>
</div>
```
Then the included contents will be shifted to the right by 5cm.

#### Font size and line height

If you find the default font size is too large or the baseline skip is too small, we can adjust it by the following:

```html
<div style="font-size:25pt; line-height:70px">
 some contents
</div>
```

[^1]: More markdwon syntax examples can be found [here](https://github.com/humrochagf/revelation/blob/main/example_slides/slides.md?plain=1).
