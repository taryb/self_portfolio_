<script>
import feather from 'feather-icons';
import ProjectHeader from '../components/projects/ProjectHeader.vue';
import ProjectGallery from '../components/projects/ProjectGallery.vue';
import ProjectInfo from '../components/projects/ProjectInfo.vue';
import ProjectRelatedProjects from '../components/projects/ProjectRelatedProjects.vue';

export default {
	name: 'Projects',
	components: {
		ProjectHeader,
		ProjectGallery,
		ProjectInfo,
		ProjectRelatedProjects,
	},
	data: () => {
		return {
			singleProjectHeader: {
				singleProjectTitle: 'WEBSCRAPE',
				singleProjectDate: 'Jul 26, 2020',
				singleProjectTag: 'Backend/Frontend',
			},
			projectImages: [
				{
					id: 1,
					title: 'SDF Cambodia',
					img: require('@/assets/images/ui-project-1.jpg'),
				},
		
			],
			projectInfo: {
				clientHeading: 'About Client',
				companyInfos: [
					{
						id: 1,
						title: 'MEF',
						details: 'Ministry of Economy and Finance',
					},
					{
						id: 2,
						title: 'Services',
						details: 'Website/Portal',
					},
					{
						id: 3,
						title: 'Website',
						details: 'http://www.sdfcambodia.org/kh/home',
					},
					{
						id: 4,
						title: 'Phone',
						details: 'N/A',
					},
				],
				objectivesHeading: 'Objective',
				objectivesDetails:
					'Webscrape',
				technologies: [
					{
						title: 'Tools & Technologies',
						techs: [
							'Python: This is a popular programming language that is commonly used for web scraping. You may have used Python libraries like BeautifulSoup and Scrapy to extract data from websites.',
							'Web Scraping Libraries: Libraries such as BeautifulSoup, Scrapy, Selenium, and PyQuery are widely used to facilitate web scraping tasks.',
							'Web Development Tools: You may have used web development tools like Inspect Element to identify the HTML elements containing the data you want to scrape.',
							'Data Storage Tools: After extracting data from websites, you may have stored it in different formats such as CSV, Excel, or JSON files, or in databases like MySQL or MongoDB.',
							'Cloud Computing Tools: You may have also leveraged cloud computing tools like Amazon Web Services or Google Cloud Platform to run your web scraping tasks more efficiently.',
							
						],
					},
				],
				projectDetailsHeading: 'Challenge',
				projectDetails: [
					{
						id: 1,
						details:
							' As someone passionate about data, I recognized the power of web scraping in collecting valuable information from websites. I researched different tools and techniques, focusing on popular Python libraries like BeautifulSoup and Scrapy, which are widely used in the web scraping community.I then embarked on a hands-on learning journey, practicing web scraping on a variety of websites to extract the desired data using Python code. This process involved identifying the HTML elements containing the data, writing code to extract it, and storing it in a format for analysis. Throughout my learning process, I faced various challenges, such as anti-scraping measures and complex website structures. However, I persevered, leveraging online resources such as forums and documentation to overcome these obstacles. As I gained more experience, I explored more advanced techniques such as APIs and handling large datasets. I also saw the potential of web scraping beyond data collection, such as building predictive models or informing business decisions. Overall, my process of learning about web scraping involved research, experimentation, and problem-solving. Through dedication and persistence, I have become proficient in this powerful tool for data analysis, and I am excited to apply my skills in various real-world contexts.',},
				],
				socialSharingsHeading: 'Share This',
				socialSharings: [
					{
						id: 1,
						name: 'Twitter',
						icon: 'twitter',
						url: 'https://twitter.com',
					},
					{
						id: 2,
						name: 'Instagram',
						icon: 'instagram',
						url: 'https://www.instagram.com/',
					},
					{
						id: 3,
						name: 'Facebook',
						icon: 'facebook',
						url: 'https://facebook.com/',
					},
					{
						id: 4,
						name: 'LinkedIn',
						icon: 'linkedin',
						url: 'https://www.linkedin.com/in/',
					},
					
				],
			},
			relatedProject: {
				relatedProjectsHeading: 'Related Projects',
				relatedProjects: [
					{
						id: 1,
						title: 'Mobile UI',
						img: require('@/assets/images/mobile-project-1.jpg'),
					},
					{
						id: 2,
						title: 'Web Application',
						img: require('@/assets/images/web-project-1.jpg'),
					},
					{
						id: 3,
						title: 'UI Design',
						img: require('@/assets/images/ui-project-2.jpg'),
					},
					{
						id: 4,
						title: 'Kabul Mobile App UI',
						img: require('@/assets/images/mobile-project-2.jpg'),
					},
				],
			},
		};
	},
	mounted() {
		feather.replace();
	},
	updated() {
		feather.replace();
	},
	methods: {},
};
</script>

<template>
	<div class="container mx-auto mt-10 sm:mt-20">
		<!-- Project header -->
		<ProjectHeader :singleProjectHeader="singleProjectHeader" />

		<!-- Project gallery -->
		<ProjectGallery :projectImages="projectImages" />

		<!-- Project information -->
		<ProjectInfo :projectInfo="projectInfo" />

		<!-- Project related projects -->
		<ProjectRelatedProjects :relatedProject="relatedProject" />
	</div>
</template>

<style scoped></style>
