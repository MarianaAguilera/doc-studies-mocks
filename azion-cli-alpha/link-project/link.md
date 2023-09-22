---
title: Link an existing project
description: Linking an existing project to run on the Azion Edge platform.
meta_tags: cli, next, javascript, astro, vue, react, edge computing
namespace: documentation_cli_link
menu_namespace: cliMenuAlpha
permalink: /documentation/products/cli/link-command/
---

See the command that enable the linking of an existing project to run on the Azion Edge platform.

---

## Link

The linking process adapts the environment for building your edge application.

### Usage

```sh
  azion link
```

### output 

Once you've initialized the linking of an existing application, the list of available modes will be output. Then, it's necessary to choose one of them.

```sh 
  Choose a mode:  [Use arrows to move, type to filter]
  > Html (Deliver)
    Javascript (Compute)
    Typescript (Compute)
    Angular (Deliver)
    Astro (Deliver)
    Hexo (Deliver)
    Next (Deliver)
```

### Optional flags

#### name

The `--name` option can be specified, but it isn't mandatory. If it isn't informed, the name of your project will be autogenerated.

#### mode

The `--mode` option can be specified, but it isn't mandatory. The expected values are `deliver` and `compute`.


#### preset

The `--preset` option can be specified, but it isn't mandatory. The expected values are:

- Html
- Javascript
- Typescript
- Angular
- Astro
- Hexo
- Next 
- React
- Vue
- static

#### help

The `--help` option displays more information about the `link` command.


---