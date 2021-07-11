# Sim Hok

A lightweight and easy-to-use library for features you probably use every day.

## Install

```sh
$ npm install simhok

# or

$ yarn add simhok
```

## Import

```javascript
const SimHok = require("simhok");
const sim = new SimHok();
```

## Usage

```javascript
const user = "sebastian";
const users = ["sebastian", "klaudia"];

sim.len(user); // number: 9
sim.len(users); // number: 2
sim.capitalize(user); // string: Sebastian
sim.upper(user); // string: SEBASTIAN
sim.lower(user); // string: sebastian

sim.startswith(user, "s"); // boolean: true
sim.startswith(user, "S"); // boolean: false
sim.endswith(user, "n"); // boolean: true

sim.split(user, [0]); // string: s
sim.split(user, [0, 2]); // string: se
sim.split(user, [3, 0]); // string: astian
sim.split(user, [0, -3]); // string: ian

let james_bond = 7;
sim.zfill(james_bond, 2); // string: 007

sim.log("test"); // "test")
```
