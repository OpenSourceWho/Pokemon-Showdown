Pokémon Showdown
========================================================================

just a fork to show how to edit some things :)

- Adding Commands
simply paste this in
```js
	'!test': true,
	test: function (target, room, user) {
		if (!this.runBroadcast()) return;
		this.sendReplyBox('<h1>This is an test command, you can edit this to make cooler things!</h1>\nYou can use html tags <u>too!</u>');
	},
```
