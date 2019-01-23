# ang-mxgraph
mxGraph definition type for angular

for using it follow this steps:

1. create  this directory in project : /assets/mxgraph
2. run npm install mxgraph
3. put this code in angular.json -> build-> options-> assets:
              {
                "glob": "**/*",
                "input": "./node_modules/mxgraph/javascript/src",
                "output": "/assets/mxgraph"
              }
4. move mxgraph resource like images and xml to /assets/mxgraph.
5. set mxBasePath = 'assets/mxgraph/' in initializing app (you can add this to build-> options->scripts as js file).
6. finally download this definition type and put it into tsconfig.json -> compilerOptions-> typeRoots like this
      "typeRoots": [
      "node_modules/@types",
      "src/mxgraphtyping"
    ]
