# On.js

	new On.extend({
		container: '#hello',

		events: [
			['click', '#say-hello', 'say-hello']
		],

		templates: {
			'say-hello': '<p>Hello, {{text}}!</p>'
		},

		sayHello: function(target, elements, data, template) {
			template(data.user, this.container);
		}
	});


	<html><body>
		<section id="hello">
			<p><button id="say-hello" data-user="octocat"></p>
		</section>
	</body></html>
