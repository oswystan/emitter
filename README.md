# emitter
A simple event emitter can be run on Browser and node

# usage

```js
let emitter = new Emitter();
function handler_hi(args) {
	console.log(args);
}
function handler_no(args) {
	console.log(args);
}

emitter.on("hi", handler_hi.bind(null));
emitter.once("no", handler_no.bind(null));
emitter.emit("hi", "tom");
emitter.emit("no", "no no no.");
emitter.emit("no", "no no no.");
emitter.aemit("hi", "tom again");

```