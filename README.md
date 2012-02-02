# On.js

	new On.extend({
		container: '#hello',

		events: [
			['click', '#say-hello', 'say-hello']
		],

		templates: {
			'say-hello': '<p>Hello, {{user}}!</p>'
		},

		sayHello: function(target, elements, data, template) {
			template(data, this.container);
		}
	});


	<html><body>
		<section id="hello">
			<p><button id="say-hello" data-user="octocat">Say Hello</button></p>
		</section>
	</body></html>
