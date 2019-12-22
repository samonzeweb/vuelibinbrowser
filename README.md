# Creating and using a vue library in a simple HTML content

## Purpose

Beeing rather a backend enginner, I struggled to build a [Vue.js](https://vuejs.org/) components library and use it in a simple HTML
file. Then I made this project as a reminder.

The library is build using [Vue Cli](https://cli.vuejs.org/).

The HTML content ( `vuelibinbrowser.html` ) is simple, and shows three way to instantiate Vue.

A key point here is that custom HTML tags have to contain lowercases and hypens, no uppercases. You can write `<hello-world>` but you can't write `<HelloWorld>` !

In `.vue` files you can use tags containing uppercases, but in standard HTML files you can't.


## Build and use

To build the library you need [node.js](https://nodejs.org/en/).

```
cd myvuelib && npm run-script build
```

Open the file `vuelibinbrowser.html` in your prefered browser. That's all.

## How the library was created

### Create a new vue project

```
npm install -g @vue/cli
vue create myvuelib
```

### Change the build type

In `package.json` replace

```
vue-cli-service build
```

with

```
vue-cli-service build --target lib --name myvuelib src/main.js
```

remove the `src/App.vue` file and the `public` folder.

### Create components

See `src/components` content. Note that `src/components/HelloWorld.vue` is not the original version.

There is nothing special here.

### Update main.js

The `src/main.js` exports only public components.

## Licence

Released under the MIT License, see LICENSE.txt for more informations.
