<script lang="ts">
	// Portfolio data
	const profile = {
		name: 'Jesse Ruth',
		title: 'Software Developement Manager',
		email: 'jesse@jesseruth.com',
		linkedin: 'https://www.linkedin.com/in/jesseruthseattle',
		github: 'https://github.com/jesseruth'
	};

	const about = `Passionate software developer with experience in full-stack development, focusing on modern web technologies. I love building efficient, user-friendly applications and contributing to open-source projects.`;

	const experience = [
		{
			title: 'Senior Developer',
			company: 'Tech Corp',
			duration: '2020 - Present',
			description: 'Led development of web applications using React and Node.js.'
		},
		{
			title: 'Junior Developer',
			company: 'Startup Inc',
			duration: '2018 - 2020',
			description: 'Built responsive websites and maintained backend services.'
		}
	];

	const education = [
		{
			degree: 'Bachelor of Science in Computer Science',
			school: 'University of Example',
			year: '2018'
		}
	];

	const skills = ['JavaScript', 'TypeScript', 'React', 'Svelte', 'Node.js', 'Python', 'Git'];

	const projects = [
		{
			name: 'Project One',
			description: 'A web app for task management.',
			link: '#'
		},
		{
			name: 'Project Two',
			description: 'An open-source library for data visualization.',
			link: '#'
		}
	];
</script>

<main class="min-h-screen bg-gradient-to-b from-black via-gray-900 to-black text-green-400 font-mono">
	<!-- Header -->
	<header class="bg-gray-800 shadow-md py-16 px-6 border-b border-green-500">
		<div class="container mx-auto text-center">
			<h1 class="text-5xl font-bold mb-4 text-green-300">{"{Jesse Ruth}"}</h1>
			<p class="text-2xl text-green-500">{profile.title}</p>
			<div class="mt-8">
				<a href="mailto:{profile.email}" class="text-green-400 hover:text-green-300 mr-6 underline text-lg">Email</a>
				<a href="{profile.linkedin}" class="text-green-400 hover:text-green-300 mr-6 underline text-lg">LinkedIn</a>
				<a href="{profile.github}" class="text-green-400 hover:text-green-300 underline text-lg">GitHub</a>
			</div>
		</div>
	</header>

	<!-- About -->
	<section class="py-20 px-6">
		<div class="container mx-auto">
			<h2 class="text-4xl font-bold mb-8 text-green-300">{"{About}"}</h2>
			<p class="text-xl leading-relaxed text-green-400 max-w-4xl mx-auto">{about}</p>
		</div>
	</section>

	<!-- Experience -->
	<section class="py-20 bg-gray-800 px-6">
		<div class="container mx-auto">
			<h2 class="text-4xl font-bold mb-8 text-green-300">{"{Experience}"}</h2>
			<div class="space-y-8">
				{#each experience as exp}
					<div class="border-l-4 border-green-500 pl-6 bg-gray-900 p-6 rounded-r-lg">
						<h3 class="text-2xl font-semibold text-green-300 mb-2">{exp.title}</h3>
						<p class="text-green-500 text-lg mb-4">{exp.company} | {exp.duration}</p>
						<p class="text-green-400 text-lg">{exp.description}</p>
					</div>
				{/each}
			</div>
		</div>
	</section>

	<!-- Education -->
	<section class="py-20 px-6">
		<div class="container mx-auto">
			<h2 class="text-4xl font-bold mb-8 text-green-300">{"{Education}"}</h2>
			<div class="space-y-6">
				{#each education as edu}
					<div class="bg-gray-900 p-6 rounded-lg border border-green-500">
						<h3 class="text-2xl font-semibold text-green-300 mb-2">{edu.degree}</h3>
						<p class="text-green-500 text-lg">{edu.school}, {edu.year}</p>
					</div>
				{/each}
			</div>
		</div>
	</section>

	<!-- Skills -->
	<section class="py-20 bg-gray-800 px-6">
		<div class="container mx-auto">
			<h2 class="text-4xl font-bold mb-8 text-green-300">{"{Skills}"}</h2>
			<div class="flex flex-wrap gap-4 justify-center">
				{#each skills as skill}
					<span class="bg-green-900 text-green-300 px-4 py-2 rounded border border-green-500 text-lg hover:bg-green-800 transition-colors">{skill}</span>
				{/each}
			</div>
		</div>
	</section>

	<!-- Projects -->
	<section class="py-20 px-6">
		<div class="container mx-auto">
			<h2 class="text-4xl font-bold mb-8 text-green-300">{"{Projects}"}</h2>
			<div class="grid md:grid-cols-2 gap-8">
				{#each projects as project}
					<div class="bg-gray-900 p-8 rounded-lg border border-green-500 hover:border-green-400 transition-colors">
						<h3 class="text-2xl font-semibold mb-4 text-green-300">{project.name}</h3>
						<p class="mb-6 text-green-400 text-lg">{project.description}</p>
						<a href="{project.link}" class="text-green-400 hover:text-green-300 underline text-lg">View Project</a>
					</div>
				{/each}
			</div>
		</div>
	</section>

	<!-- Contact -->
	<section class="py-20 bg-black text-green-400 border-t border-green-500 px-6">
		<div class="container mx-auto text-center">
			<h2 class="text-4xl font-bold mb-8 text-green-300">{"{Contact}"}</h2>
			<p class="text-xl mb-8">Get in touch!</p>
			<a href="mailto:{profile.email}" class="bg-green-600 hover:bg-green-700 text-black px-8 py-4 rounded border border-green-500 text-lg font-semibold transition-colors">Email Me</a>
		</div>
	</section>
</main>
