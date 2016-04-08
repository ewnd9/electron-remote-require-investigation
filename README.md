## Description

`index.html` (renderer) contains code requiring dependency 'a' which try to require both via
default require and remote require its own dependecy 'b' (`node_modules/a/node_modules/b`)
and top level dependency 'c' (`node_modules/c`)

Output of log inside devtools

```
b is required
b is not remote required Error: Cannot find module 'b'(…)(anonymous function)
c is required
c is remote required
```

## Install

```
$ npm install
```

## Usage

```
$ npm start
```
