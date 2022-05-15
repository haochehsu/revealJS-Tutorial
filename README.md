# Reveal.js Tutorial

This is a tutorial of utilizing the [`reveal.js` framework](https://revealjs.com/) with markdown by using the [reveal-md](https://github.com/webpro/reveal-md) tool. Comparing to [Beamer](https://www.overleaf.com/learn/latex/Beamer) which create PDF slides, `reveal.js` creates brower-based slides. A comparison between the two tools is [here](https://www.maths.dur.ac.uk/users/s.m.fearn/blog/2020/revealjs/).

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
