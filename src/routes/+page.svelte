<script lang="ts">
	// Portfolio data
	const profile = {
		name: 'Jesse Ruth',
		title: 'Software Developer',
		email: 'jesse@jesseruth.com',
		linkedin: 'https://linkedin.com/in/jesseruth',
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

<main class="min-h-screen bg-gray-100 text-gray-900">
	<!-- Header -->
	<header class="bg-white shadow-md py-8">
		<div class="container mx-auto px-4 text-center">
			<h1 class="text-4xl font-bold mb-2">{profile.name}</h1>
			<p class="text-xl text-gray-600">{profile.title}</p>
			<div class="mt-4">
				<a href="mailto:{profile.email}" class="text-blue-600 hover:underline mr-4">Email</a>
				<a href="{profile.linkedin}" class="text-blue-600 hover:underline mr-4">LinkedIn</a>
				<a href="{profile.github}" class="text-blue-600 hover:underline">GitHub</a>
			</div>
		</div>
	</header>

	<!-- About -->
	<section class="py-12">
		<div class="container mx-auto px-4">
			<h2 class="text-3xl font-bold mb-6">About</h2>
			<p class="text-lg leading-relaxed">{about}</p>
		</div>
	</section>

	<!-- Experience -->
	<section class="py-12 bg-white">
		<div class="container mx-auto px-4">
			<h2 class="text-3xl font-bold mb-6">Experience</h2>
			<div class="space-y-6">
				{#each experience as exp}
					<div class="border-l-4 border-blue-500 pl-4">
						<h3 class="text-xl font-semibold">{exp.title}</h3>
						<p class="text-gray-600">{exp.company} | {exp.duration}</p>
						<p class="mt-2">{exp.description}</p>
					</div>
				{/each}
			</div>
		</div>
	</section>

	<!-- Education -->
	<section class="py-12">
		<div class="container mx-auto px-4">
			<h2 class="text-3xl font-bold mb-6">Education</h2>
			<div class="space-y-4">
				{#each education as edu}
					<div>
						<h3 class="text-xl font-semibold">{edu.degree}</h3>
						<p class="text-gray-600">{edu.school}, {edu.year}</p>
					</div>
				{/each}
			</div>
		</div>
	</section>

	<!-- Skills -->
	<section class="py-12 bg-white">
		<div class="container mx-auto px-4">
			<h2 class="text-3xl font-bold mb-6">Skills</h2>
			<div class="flex flex-wrap gap-2">
				{#each skills as skill}
					<span class="bg-blue-100 text-blue-800 px-3 py-1 rounded-full">{skill}</span>
				{/each}
			</div>
		</div>
	</section>

	<!-- Projects -->
	<section class="py-12">
		<div class="container mx-auto px-4">
			<h2 class="text-3xl font-bold mb-6">Projects</h2>
			<div class="grid md:grid-cols-2 gap-6">
				{#each projects as project}
					<div class="bg-white p-6 rounded-lg shadow-md">
						<h3 class="text-xl font-semibold mb-2">{project.name}</h3>
						<p class="mb-4">{project.description}</p>
						<a href="{project.link}" class="text-blue-600 hover:underline">View Project</a>
					</div>
				{/each}
			</div>
		</div>
	</section>

	<!-- Contact -->
	<section class="py-12 bg-gray-800 text-white">
		<div class="container mx-auto px-4 text-center">
			<h2 class="text-3xl font-bold mb-6">Contact</h2>
			<p class="text-lg mb-4">Get in touch!</p>
			<a href="mailto:{profile.email}" class="bg-blue-600 hover:bg-blue-700 text-white px-6 py-3 rounded-lg">Email Me</a>
		</div>
	</section>
</main>
