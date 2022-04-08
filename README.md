# My Marp workspace

## Install
1. Run `npm install`
2. Install the recommended VSCode workspace extensions (to preview the slides in VSCode)

## Generate slides (png)

1. Create a `.md` file within a `slides` folder 
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

