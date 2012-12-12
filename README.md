Usage:

    node watcher.js basePath [--pjs-watch path]+ [--pjs args..]

  - `basePath` Specify a folder to watch changes.
  - `--pjs-watch` When files inside path update, regenerate .pjs in basePath.
  - `--pjs` All arguments following are forwarded to cpp.

Example:

    node watcher.js ./doc/ --pjs-watch inc/ --pjs -D DEBUG

Watch files in ./doc/, update ./doc/*.pjs when ./doc/inc/* change.