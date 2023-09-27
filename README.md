# React Mobx SSR (Server Side Rendered) Boilerplate

Hey developer 👋

This is a repository with an example of a base application that can scale, using [Mobx](https://mobx.js.org/README.html) as state manager. 

Some considerations were done while creating this boilerplate:
- using classes for modules (OOP) instead of functional programming (could be refactored, but this is personal preference)
- Interface based implementation (easy to swap modules at any time, different modules between server and client side if required)
- used [InversifyJS](https://inversify.io/) for inversion of control
- made a simple [webpack](https://webpack.js.org/) configuration

## Developing
Install dependencies:
```bash
npm i
```

Start developing:
```bash
npm run dev
```

Production build
```bash
npm run build
```

Production server
```bash
npm run start
```

## To Do:
- better styling (this is mainly showcasing architecture, not UI)
- extract layout to file for better customization (`index.ejs`)
- ability to set `basename` by http request headers (`x-basename`) - good for ssr micro-frontends
- replace `<Head>` custom implementation with [react-helmet](https://github.com/nfl/react-helmet)
