# My Marp workspace

## Install
1. Run `npm install`
2. Install the recommended VSCode workspace extensions (to preview the slides in VSCode)

## Generate slides (png)

1. Create a `slides` folder in the root
2. Create a `.md` file within the `slides` folder 
3. Write your markdown slides following [marp syntax](https://marpit.marp.app/markdown)
2. Run `npm run export`
3. The resulting .pngs can be located in `_output`

To enable Marp in a `.md` file, make sure to add the following at the top of the document:

```yml
---
marp: true
---
```

You can also add other properties to customize your slides:

```yml
---
marp: true
paginate: true
theme: theme-yellow
size: 4:5
footer: paulasantamaria.com                                @pau.codes
---
```

> This properties are called "directives". Learn more about them [here](https://marpit.marp.app/directives)

# Sample .md file

```
<!-- ./slides/my-carousel.md -->

---
marp: true
paginate: true
theme: theme-blue-dark
size: 4:5
footer: @pau.codes
header: TypeScript Gamified
---

# First slide title

![](./assets/some-pic.png)

---

# Second slide title

```ts
  console.log('some code');
\``` 
<!-- Ignore the bar. I had to add it to avoid breaking the README's markdown -->

---

<!-- Use html elements with css to override the default styles defined in the theme -->
<div class="final-slide">

# Final slide
## Call to action

</div>

```

# Tools

Tools used in this workspace:

- [Marp CLI](https://github.com/marp-team/marp-cli)
- [Marp VSCode extension](https://github.com/marp-team/marp-vscode)
- Syntax theme: Atom One Dark by Daniel Gamage
