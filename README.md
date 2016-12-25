# typescript-slimline
The simplest possible(?) typescript app written to help me understand how the build process works.

Typescript needs to be transpliled to javascript so that browsers support it. So I've installed typescript, webpack and ts-loader using npm. ts-loader is a loader for webpack that does the transpiling. tsconfig is a file for the typescript transpiler options, but it's pretty much blank so I presume ts-loader is doing its own thing.

To run this:
npm install
npm run webpack
npm start
Then go to http://127.0.0.1:8080

## maybe it could have been simpler
You can run the transpiler manually, but I didn't look into it too much. Seems like you could manually transpile. The following command does transpile, but only to node.
node node_modules/typescript/bin/tsc ./src/app.ts
