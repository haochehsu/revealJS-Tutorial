# Reveal.js Tutorial

This is a tutorial of utilizing the [reveal.js framework](https://revealjs.com/) with [markdown](https://www.markdownguide.org/) by using the [reveal-md](https://github.com/webpro/reveal-md) tool. Comparing to [Beamer](https://www.overleaf.com/learn/latex/Beamer) which creates PDF slides with `TeX`, `reveal.js` creates brower-based slides (convertable to PDF) with Javascript + HTML + CSS. A comparison between the two tools is [here](https://www.maths.dur.ac.uk/users/s.m.fearn/blog/2020/revealjs/).

- Workflow: Edit the slides in markdwon → convert to HTML slides.

🔖 An example is demonstrated [here](https://www.haochehsu.com/slides/revealJS/index.html). It's markdown file is [here](https://github.com/howardhsumail/revealJS-Tutorial/tree/main/Example).

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

Drag the markdown (`.md`) file into the Terminal to obtain the file path.

- Live view the slides

```shell
reveal-md yourSlides.md -w
```

 The terminal will retruns the following message: `Reveal-server started at http://localhost:xxxx`. If the browser does not pop up, paste `http://localhost:xxxx` into the browser to start live editing.

### Markdown

Most of the time, we need to rely on HTML + CSS code to control the style and the animation of the slides, so [VS Code](https://code.visualstudio.com/) is the recommanded editor. For plain markdwon file, [Typora](https://typora.io/) is recommanded.
