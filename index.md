<!doctype html>
<html>
	<head>
		<meta charset="utf-8">
		<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">

		<title>reveal.js</title>

		<link rel="stylesheet" href="dist/reset.css">
		<link rel="stylesheet" href="dist/reveal.css">
		<link rel="stylesheet" href="dist/theme/black.css" id="theme">

		<!-- Theme used for syntax highlighted code -->
		<link rel="stylesheet" href="plugin/highlight/monokai.css" id="highlight-theme">
	</head>
	<body>
		<div class="reveal">
			<div class="slides">
				<section>Slide 1</section>
				<section>Slide 2</section>
			</div>
		</div>

		<script src="dist/reveal.js"></script>
		<script src="plugin/notes/notes.js"></script>
		<script src="plugin/markdown/markdown.js"></script>
		<script src="plugin/highlight/highlight.js"></script>
		<script>
			// More info about initialization & config:
			// - https://revealjs.com/initialization/
			// - https://revealjs.com/config/
			Reveal.initialize({
				hash: true,
				multiplex: {
					// Example values. To generate your own, see the socket.io server instructions.
					secret: null, // null so the clients do not have control of the master presentation
					id: 'ba3de982323c19d6', // id, obtained from socket.io server
					url: 'https://reveal-multiplex.glitch.me/1948' // Location of socket.io server
				},

				// Don't forget to add the dependencies
				dependencies: [
					{ src: 'https://reveal-multiplex.glitch.me/socket.io/socket.io.js', async: true },
					{ src: 'https://reveal-multiplex.glitch.me/client.js', async: true }
				],
				// Learn about plugins: https://revealjs.com/plugins/
				plugins: [ RevealMarkdown, RevealHighlight, RevealNotes ]
			});
		</script>
	</body>
</html>
