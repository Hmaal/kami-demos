## browse source code

- [basic](src/basic) - sprite rendering
- [assets](src/assets) - asset preloading
- [shaders](src/shaders) - including GLSL source in your game
- [shockwave](src/shockwave) - a shockwave shader example, using post-processing
- [normals](src/normals) - a more advanced normal-mapping shader for 2D graphics

## view the demos

- [basic](http://mattdesl.github.io/kami-demos/release/basic.html)
- [assets](http://mattdesl.github.io/kami-demos/release/assets.html)
- [shaders](http://mattdesl.github.io/kami-demos/release/shaders-brfs.html)
- [shockwave](http://mattdesl.github.io/kami-demos/release/shockwave.html)
- [normals](http://mattdesl.github.io/kami-demos/release/normals.html)

## modifying & building the demos

[Install node.js](http://nodejs.org/), it should come bundled with NPM. Then `cd` to this directory and run the following to build the demos:

```
npm install
node build
```

This will write HTML and JS files to the `release` folder. Then you should serve up the `release` folder and browse it on your localhost. To watch the source folder for changes, you can use nodemon and the following command:

```
nodemon --watch src -e js,html,vert,frag build.js
```