# bs-chokidar

[BuckleScript](https://bucklescript.github.io) bindings for [chokidar](https://github.com/paulmillr/chokidar).

# Usage

```reasonml
let watcher = Chokidar.watch(".", ());
let doit = (s:string) => Js.log(s);
Chokidar.on(watcher, "change", doit);
Chokidar.close(watcher, ());
```

# Developers section

First and formost, configure your environment with `npm install`.

Specific BuckleScript aliases (`clean`, `build`, `watch`, `test`...) are defined
in the `package.json` file to be used with `npm run [alias]`.
