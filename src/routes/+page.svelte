<script lang="ts">
	// Portfolio data
	const profile = {
		name: 'Jesse Ruth',
		title: 'Team Manager – CXP Portfolio (Strategic Investments)',
		email: 'jesse@jesseruth.com',
		linkedin: 'https://www.linkedin.com/in/jesseruthseattle',
		github: 'https://github.com/jesseruth'
	};

	const about = `Experienced software development manager and full-stack engineer with over 15 years in technology, specializing in web development, DevOps, and operational tooling. Passionate about building scalable applications, mentoring teams, and driving innovation in cloud-native environments.`;

	const experience = [
		{
			title: 'Software Development Manager – CXP Portfolio (Strategic Investments)',
			company: 'Expeditors',
			duration: 'Aug 2025 – Present',
			location: 'Greater Seattle Area',
			description: 'Lead the Risk Management Development team, driving delivery of the modern Claims and ECIB Insurance platform.'
		},
		{
			title: 'Senior Developer',
			company: 'Expeditors',
			duration: 'Jan 2023 – Aug 2025',
			location: 'Greater Seattle Area',
			description: ''
		},
		{
			title: 'Developer III',
			company: 'Expeditors',
			duration: 'May 2022 – Jan 2023',
			location: 'Seattle, WA',
			description: ''
		},
		{
			title: 'Developer II',
			company: 'Expeditors',
			duration: 'Sep 2021 – May 2022',
			location: 'Seattle, WA',
			description: ''
		},
		{
			title: 'Senior Member Of Technical Staff – DevOps Portal',
			company: 'Oracle',
			duration: 'Mar 2020 – Aug 2021',
			location: 'Seattle, WA',
			description: 'Delivered large-scale features, mentored junior engineers, and collaborated with UI/UX teams to enhance user experience. Served as Technical Subject Matter Expert and advocate for customer-focused solutions. Built features supporting custom notifications, user profiles, custom calendars, and timeline visualizations. Migrated build pipelines from TeamCity to internal build services using Node.js, Yarn, Maven, and Makefiles. Grafana Subject Matter Expert: Launched an internal tool enabling teams to manage dashboards via Terraform across multiple regions. Developed migration scripts, code sample repositories, and wikis to establish best practices and templating standards.'
		},
		{
			title: 'Senior Member Of Technical Staff – Operations Tooling',
			company: 'Oracle',
			duration: 'Nov 2018 – Mar 2020',
			location: 'Seattle, WA',
			description: 'Developed internal operational tools and web applications using React, TypeScript, and Java. Implemented and designed an extensible UI/UX Framework. Migrated legacy codebases to TypeScript, significantly increasing test coverage. Coached engineers on complex JavaScript problems and development patterns.'
		},
		{
			title: 'SDE – Operations Tooling',
			company: 'Oracle',
			duration: 'Dec 2017 – Nov 2018',
			location: 'Seattle, WA',
			description: 'Lead Web Engineer: Built and maintained internal web apps for distributed cloud-native alerting systems. Designed and implemented a React/TypeScript application, delivering MVP ahead of schedule to serve thousands of engineers hourly. Back-End Contributor: Influenced major features of the Java JAX-RS REST Web API. Migrated class-based components to functional hooks and implemented state management using Redux.'
		},
		{
			title: 'Part-Time Adjunct Faculty',
			company: 'Bellevue College',
			duration: 'Sep 2018 – Dec 2018',
			location: 'Bellevue, WA',
			description: 'Year Up Instructor: Taught "Introduction to Web Development" to underserved young adults. Instructed students on HTML, CSS, and JavaScript fundamentals. Mentored students on business communication and workplace culture.'
		},
		{
			title: 'Web Development Engineer',
			company: 'Amazon Web Services (AWS)',
			duration: 'Oct 2016 – Nov 2017',
			location: 'Greater Seattle Area',
			description: 'Front-end MVC web application developer responsible for design, testing, deployment, and maintenance. Utilized HTML, SASS/CSS, JavaScript (Knockout.js, jQuery), and C#. Leveraged the AWS Toolchain extensively, alongside Git, Gulp, and Jenkins. Collaborated in an Agile environment with product managers, marketing, and UX designers.'
		},
		{
			title: 'Business Analyst',
			company: 'Amazon Web Services (AWS)',
			duration: 'Sep 2015 – Oct 2016',
			location: 'Greater Seattle Area',
			description: 'Identified process improvement opportunities and automated business processes using Python, Pandas, and Selenium. Analyzed data using AWS Redshift and created dashboards as a Tableau Server Administrator. Managed SharePoint administration and supported stakeholders with MS Excel automation.'
		},
		{
			title: 'Risk Management Systems Development Manager',
			company: 'Expeditors (Previous Tenure)',
			duration: 'Jul 2015 – Aug 2015',
			location: 'Greater Seattle Area',
			description: 'Served as business stakeholder for the development of Insurance and Claims systems. Directed validation and QA for continuous development cycles. Managed BI, Analytics, and Tableau ad-hoc reporting.'
		},
		{
			title: 'Business Analytics Developer – Risk Management & Insurance',
			company: 'Expeditors (Previous Tenure)',
			duration: 'Dec 2012 – Jul 2015',
			location: '',
			description: 'First full-time Analytics Developer for the department, supporting 70+ specialists in insurance, security, and finance. Led the acquisition and installation of Tableau Server; acted as administrator and lead trainer. Migrated and refactored a large base of legacy reports into interactive workbooks. Utilized Python (Pandas/IPython) for data wrangling and exploratory analysis. Developed reporting for revenue, accruals, reserves, and claims management. Global Secure Services: Researched IoT product offerings using Google APIs, Django, GeoDjango, and PostGIS.'
		},
		{
			title: 'Cargo Claims Specialist',
			company: 'Expeditors (Previous Tenure)',
			duration: 'Feb 2011 – Dec 2012',
			location: '',
			description: 'Managed cargo loss claims and insurance adjusting for high-revenue global accounts. Designed "Riskapedia," a department wiki to standardize processes across teams. Developed systems to manage claim payments and created financial auditing tools. Trained global locations on freight receiving techniques and data analysis.'
		},
		{
			title: 'Vessel Boarding Agent',
			company: 'B.R. Anderson & Co.',
			duration: 'Feb 2007 – Feb 2011',
			location: 'Seattle, WA',
			description: 'Developed a Line of Business (LOB) application using Lotus Approach to improve efficiency. Created local databases for document management and compliance reporting. Coordinated harboring of ocean vessels and acted as a liaison between government and industry.'
		},
		{
			title: 'Petty Officer Third Class',
			company: 'US Navy',
			duration: 'Jan 1997 – Jan 2001',
			location: '',
			description: 'Boatswain\'s Mate: Deployed globally; gained expertise in maintenance, welding, and industrial skills.'
		}
	];

	const education = [
		{
			degree: 'Bachelor of Fine Arts (B.F.A.), Art & Technology',
			school: 'Youngstown State University',
			year: '2001 – 2005',
			description: 'Activities and societies: I worked in the costume shop helping to design and fabricate costumes and I worked one year in the ceramic department where I helped to create glazes, make clay and assist with general duties. I attended YSU on my GI Bill after completing a four year enlistment in the Navy. My awarded degree is a Bachelor of Fine Arts (B.F.A.), but by focusing on Art & Technology I was able to take a variety of classes in digital arts and computer science along with a complete battery of traditional and fine arts. The biggest take away from a BFA for me was the concept of an algorithm as a step-by-step procedure for creation. While algorithms are used for calculation, data processing, and automated reasoning they are also at home in the act of screen printing, photography, and ceramics.'
		},
		{
			degree: 'Certificate in Java Programming',
			school: 'University of Washington',
			year: 'Oct 2021 – Jun 2022',
			description: 'Acquired a comprehensive foundation in software engineering, mastering core Java syntax, advanced object-oriented programming principles, and industry-standard techniques for building robust, scalable applications.'
		}
	];

	const skills = [
		'JavaScript', 'TypeScript', 'React', 'Redux', 'Node.js', 'Yarn', 'Maven', 'Terraform', 'Grafana', 'Java', 'HTML', 'CSS', 'SASS', 'Knockout.js', 'jQuery', 'C#', 'Python', 'Pandas', 'Selenium', 'AWS Redshift', 'Tableau', 'Django', 'GeoDjango', 'PostGIS', 'Git', 'Gulp', 'Jenkins', 'AWS Toolchain', 'Makefiles', 'TeamCity'
	];

	const projects = [
		{
			name: 'Grafana Dashboard Management Tool',
			description: 'Internal tool enabling teams to manage dashboards via Terraform across multiple regions.',
			link: '#'
		},
		{
			name: 'Cloud-Native Alerting System',
			description: 'React/TypeScript application serving thousands of engineers hourly.',
			link: '#'
		},
		{
			name: 'Riskapedia Wiki',
			description: 'Department wiki to standardize processes across teams.',
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
						<p class="text-green-500 text-lg mb-4">{exp.company} | {exp.duration}{exp.location ? ` | ${exp.location}` : ''}</p>
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
						<p class="text-green-500 text-lg mb-4">{edu.school}, {edu.year}</p>
						<p class="text-green-400 text-lg">{edu.description}</p>
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
						<p class="text-green-400 text-lg">{project.description}</p>
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
