<script>
	let timeline = [
		{
			year: '1943',
			events: [
				{
					title: 'Birth of Neural Networks',
					description:
						'In 1943, McCulloch and Pitts proposed the artificial neuron model, pioneering neural networks and laying groundwork for modern AI and machine learning.',
					link: ''
				}
			]
		},
		{
			year: '1945',
			events: [
				{
					title: 'ENIAC',
					description:
						'The Electronic Numerical Integrator and Computer (ENIAC) was completed, marking one of the earliest general-purpose computers.',
					link: ''
				}
			]
		},
		{
			year: '1950',
			events: [
				{
					title: 'Turing Test',
					description:
						"Alan Turing proposed the Turing Test as a criterion of intelligence, a test of a machine's ability to exhibit intelligent behavior equivalent to, or indistinguishable from, that of a human.",
					link: ''
				}
			]
		},
		{
			year: '1954',
			events: [
				{
					title: 'First Machine Translation',
					description:
						'The first demonstration of machine translation was performed by IBM on a Russian-English translation system.',
					link: ''
				}
			]
		},
		{
			year: '1956',
			events: [
				{
					title: 'Dartmouth AI Workshop',
					description:
						'The Dartmouth Conference, organized by John McCarthy, Marvin Minsky, Nathaniel Rochester, and Claude Shannon, is considered the founding event of artificial intelligence as a field.',
					link: ''
				}
			]
		},
		{
			year: '1957',
			events: [
				{
					title: 'Perceptron',
					description:
						'Frank Rosenblatt developed the Perceptron, an early type of artificial neural network.',
					link: ''
				}
			]
		},
		{
			year: '1966',
			events: [
				{
					title: 'ELIZA chatbot',
					description:
						'Joseph Weizenbaum created ELIZA, an early natural language processing computer program that demonstrated the superficiality of communication between humans and machines.',
					link: ''
				}
			]
		},
		{
			year: '1970',
			events: [
				{
					title: 'First AI Winter',
					description:
						'The first AI winter began, a period of reduced funding and interest in artificial intelligence research.',
					link: ''
				}
			]
		},
		{
			year: '1975',
			events: [
				{
					title: 'Relu Activation Function',
					description:
						'The Rectified Linear Unit (ReLU) activation function was introduced, which later became a standard in deep learning models.',
					link: ''
				}
			]
		},
		{
			year: '1986',
			events: [
				{
					title: 'Backpropagation Breakthrough',
					description:
						'David Rumelhart, Geoffrey Hinton, and Ronald Williams published a paper on the backpropagation algorithm, which significantly advanced neural network training.',
					link: ''
				}
			]
		},
		{
			year: '1990',
			events: [
				{
					title: 'Second AI Winter & ML Rise',
					description:
						'The second AI winter occurred, but machine learning began to rise in prominence with the development of new algorithms and increased computational power.',
					link: ''
				}
			]
		},
		{
			year: '2006',
			events: [
				{
					title: 'Deep Learning Resurgence',
					description:
						'Geoffrey Hinton and his team demonstrated the power of deep learning with their work on deep belief networks, leading to a resurgence of interest in neural networks.',
					link: ''
				}
			]
		},
		{
			year: '2012',
			events: [
				{
					title: 'AlexNet',
					description:
						'AlexNet, developed by Alex Krizhevsky, Ilya Sutskever, and Geoffrey Hinton, won the ImageNet Large Scale Visual Recognition Challenge, showcasing the power of deep convolutional neural networks.',
					link: ''
				}
			]
		},
		{
			year: '2017',
			events: [
				{
					title: 'Transformer',
					description:
						'The Transformer model, introduced by Vaswani et al., revolutionized natural language processing by enabling more efficient training of large-scale models.',
					link: ''
				}
			]
		},
		{
			year: '2022',
			events: [
				{
					title: 'ChatGPT',
					description:
						'OpenAI released ChatGPT, a large language model based on the GPT-3 architecture, capable of generating human-like text and engaging in conversational interactions.',
					link: ''
				}
			]
		}
	];
</script>

<main class="relative flex flex-col justify-center">
	<h1 class="text-3xl font-bold text-center mt-4 mb-12">Timeline AI</h1>
	<div class="max-w-screen-sm mx-auto">
		{#each timeline as t}
			<div class="flex relative space-x-4 mb-4">
				<div class="font-bold">
					{t.year}
				</div>
				{#each t.events as e}
					<div>
						<a href={e.link} class="text-gray-700 hover:text-gray-900">{e.title}</a>
						<p class="text-sm text-gray-500">{e.description}</p>
					</div>
				{/each}
			</div>
		{/each}
	</div>
</main>
