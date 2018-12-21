Pokémon Showdown
========================================================================

just a fork to show how to edit some things :)

- Adding Commands
simply paste this in chat-commands.js
```js
	'!test': true,
	test: function (target, room, user) {
		if (!this.runBroadcast()) return;
		this.sendReplyBox('<h1>This is an test command, you can edit this to make cooler things!</h1>\nYou can use html tags <u>too!</u>');
	},
```

- The command basics
How is a reply made you ask?
well simply you need to call `sendReplyBox`
example: `this.sendReplyBox('Test!');`

How do you create a new command?
first we will go on how it's called in the chat
simply in our first example on the first line you'll see `'!test': true,`
the first arg is suppose how can you call the command in the chat
so if i made it `'!hello': true,` if i said `!hello` in the chat the function is called
now we will go to responses/etc.
so before you write responses such as sending replys you need to enter this `commandName: function (target, room, user) {` (change commandName to the name of your certain command)
now just to detect this is being ran in the chat we need to also put `if (!this.runBroadcast()) return;`

