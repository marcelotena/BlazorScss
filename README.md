# Blazor .NET 8 with SASS compiling and browser JS/CSS injection (without reload)

Blazor project with automatic compiling of .scss and .js files from "src" folder.

File src/bundle.js is used by parcel-bundler as entry point, node_modules packages can also be included without need of a full path (see .sassrc).

Blazor's scoped CSS functionality still works as usual, with standard .css files.

## Development dependencies
- Local Node and NPM: "16.14.2" and "8.12.2"
- parcel-bundler: 1.12.5
- sass: 1.75.0

## Building assets

Parcel-bundler reads from "src/bundle.js" and outputs "bundle.css" and "bundle.js" files into "wwwroot/dist/" folder.

To run development file watch task:
```sh
npm run watch
```

To run build task (minifying output files):
```sh
npm run build
```