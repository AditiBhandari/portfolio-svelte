<script>
	import Nav from "./components/Nav.svelte";
	import StoryCard from "./components/StoryCard.svelte";

	let sectionList = {
		sections: [
			{
				page: "home",
				section: "work",
				title: "my favourite work",
				text: "",
				stories: [
					{
						link: "https://graphics.reuters.com/PARALYMPICS-2022/EQUIPMENT/dwpkrlmnrvm/",
						slug: "Culture",
						title: "Built to win",
						description:
							"The adaptive sports tools powering the 2022 Winter Paralympics.",
						publication: "Reuters",
						year: 2022,
						thumbnail:
							"https://graphics.reuters.com/PARALYMPICS-2022/EQUIPMENT/dwpkrlmnrvm/cdn/images/reuters-graphics.jpg",
					},
					{
						link: "https://graphics.reuters.com/MYANMAR-POLITICS/zjpqkkoaqpx/",
						slug: "Conflict",
						title: "Myanmar protest deaths",
						description:
							"The tragedy still unfolding in Myanmar, told through the profiles of seven people who died after the military cracked down on protests after the 2021 coup.",
						publication: "Reuters",
						year: 2021,
						thumbnail:
							"https://graphics.reuters.com/MYANMAR-POLITICS/zjpqkkoaqpx/img/share.png",
					},
					{
						link: "https://graphics.reuters.com/GLOBAL-RACE/BTS-FANS/nmopajgmxva/",
						slug: "Culture",
						title: "BTS ARMY's fundraising power",
						description:
							"Interviewed BTS fans and experts, created the data graphics and designed and built the page. It won an Award of Excellence at the SND: Best of Digital News Design awards, and BTS fans showed their love on Twitter.",
						publication: "Reuters",
						year: 2020,
						thumbnail:
							"https://graphics.reuters.com/GLOBAL-RACE/BTS-FANS/nmopajgmxva/img/share-card.png",
					},
				],
			},
			{
				page: "home",
				section: "projects",
				title: "my favourite projects",
				text: "",
				stories: [
					{
						workSection: "resources",
						workFeature: "faveProjects",
						link: "https://github.com/AditiBhandari/south-asia-data-sources",
						slug: null,
						title: "South Asia Data Sources",
						description:
							"Growing list of govermental, research and other sources of data about India and the South Asia subcontinent.",
						publication: null,
						year: null,
						thumbnail:
							"https://aditibhandari.github.io/img/github-repo.webp",
					},
					{
						workSection: "resources",
						workFeature: "faveProjects",
						link: "https://github.com/AditiBhandari/data-journalism-early-career-tips",
						slug: null,
						title: "NICAR 18 Early Career Tips",
						description:
							"A list of community groups and resources for young and early-career data journalists. Made with Madi Alexander for <a class='sample_text_link' href='https://twitter.com/search?q=aditihbhandari%20%23NICAR18&amp;src=typd' target='_blank' rel='noopener noreferrer'>#NICAR18</a>",
						publication: null,
						year: null,
						thumbnail:
							"https://aditibhandari.github.io/img/github-repo.webp",
					},
					{
						workSection: "lightning talk",
						workFeature: "faveProjects",
						link: "https://aditibhandari.github.io/nicar17-slides/",
						slug: null,
						title: "Self-Care For Nerds",
						description:
							"Pitched and gave a lightning talk at #NICAR17 about physical self-care as a developer, journalist, or just someone who sits at a computer all day. Here are my slides and speaker notes.",
						publication: null,
						year: null,
						thumbnail:
							"https://aditibhandari.github.io/img/github-repo.webp",
					},
				],
			},
			{
				page: "work",
				section: "digitalWork",
				title: "digital work",
				text: "I design page and/or work on graphics depending on the project. Always looking for opportunities to templatise work and document for future use. Lately been making a more concerted effort to make projects accessible while covering, and wrapping it into documentation and training",
				stories: [
					{
						workSection: "allDigitalWork",
						workFeature: "faveWork",
						link: "https://graphics.reuters.com/PARALYMPICS-2022/EQUIPMENT/dwpkrlmnrvm/",
						slug: "Culture",
						title: "Built to win",
						description:
							"The adaptive sports tools powering the 2022 Winter Paralympics",
						publication: "Reuters",
						year: 2022,
						thumbnail:
							"https://graphics.reuters.com/PARALYMPICS-2022/EQUIPMENT/dwpkrlmnrvm/cdn/images/reuters-graphics.jpg",
					},
					{
						workSection: "allDigitalWork",
						workFeature: "faveWork",
						link: "https://graphics.reuters.com/GLOBAL-RACE/BTS-FANS/nmopajgmxva/",
						slug: "Culture",
						title: "BTS ARMY's fundraising power",
						description:
							"Interviewed BTS fans and experts, created the data graphics and designed and built the page. It won an Award of Excellence at the SND: Best of Digital News Design awards, and BTS fans showed their love on Twitter.",
						publication: "Reuters",
						year: 2020,
						thumbnail:
							"https://graphics.reuters.com/GLOBAL-RACE/BTS-FANS/nmopajgmxva/img/share-card.png",
					},
					{
						workSection: "allDigitalWork",
						workFeature: "faveWork",
						link: "https://graphics.reuters.com/MYANMAR-POLITICS/zjpqkkoaqpx/",
						slug: "Conflict",
						title: "Myanmar protest deaths",
						description:
							"The tragedy still unfolding in Myanmar, told through the profiles of seven people who died after the military cracked down on protests after the 2021 coup.",
						publication: "Reuters",
						year: 2021,
						thumbnail:
							"https://graphics.reuters.com/MYANMAR-POLITICS/zjpqkkoaqpx/img/share.png",
					},
					{
						workSection: "allDigitalWork",
						workFeature: "faveWork",
						link: "https://graphics.reuters.com/ETHIOPIA-CONFLICT/EXPULSIONS/yzdpxmqyavx/index.html",
						slug: "Conflict",
						title: "Witnesses to slaughter",
						description:
							"Reuters has maps the violence in western Tigray by drawing on more than 120 interviews in Ethiopia and Sudan.",
						publication: "Reuters",
						year: 2021,
						thumbnail:
							"https://graphics.reuters.com/ETHIOPIA-CONFLICT/EXPULSIONS/yzdpxmqyavx/img/share.png",
					},
					{
						workSection: "allDigitalWork",
						workFeature: "faveWork",
						link: "https://graphics.reuters.com/ETHIOPIA-CONFLICT/xklpyjmndvg/index.html",
						slug: "Conflict",
						title: "The conflict in Ethiopia",
						description:
							"Compiled reporting and photos from Reuters’ East Africa bureau and collaborated with a correspondent to recreate and provide context on how the Ethiopia conflict in the northern state of Tigray unfolded over the course of a month.",
						publication: "Reuters",
						year: 2020,
						thumbnail:
							"https://graphics.reuters.com/ETHIOPIA-CONFLICT/xklpyjmndvg/img/share.png",
					},
					{
						workSection: "allDigitalWork",
						workFeature: "faveWork",
						link: "https://graphics.reuters.com/HEALTH-CORONAVIRUS/WUHAN/rlgpdkxzavo/index.html",
						slug: "COVID",
						title: "Reopening a megacity",
						description:
							"Designed and built a scrolly reconstruction of how Wuhan gradually reopened its doors to the public. Illustrated an isometric city, recreated a Chinese health status checker and visualized China's coronavirus cases and testing.",
						publication: "Reuters",
						year: 2020,
						thumbnail:
							"https://graphics.reuters.com/HEALTH-CORONAVIRUS/WUHAN/rlgpdkxzavo/images/share-card.png",
					},
					{
						workSection: "allDigitalWork",
						workFeature: "",
						link: "https://graphics.reuters.com/CHINA-CRASH/znvneqennpl/index.html",
						slug: "Breaking news",
						title: "Plane crash in China",
						description:
							"A China Eastern Airlines passenger jet with 132 people on board crashed in the mountains of southern China en route from the southwestern city of Kunming to Guangzhou, on the east coast.",
						publication: "Reuters",
						year: 2022,
						thumbnail:
							"https://graphics.reuters.com/CHINA-CRASH/znvneqennpl/cdn/images/reuters-graphics.jpg",
					},
					{
						workSection: "allDigitalWork",
						workFeature: "",
						link: "https://graphics.reuters.com/TONGA-VOLCANO/znpnejbjovl/",
						slug: "Breaking news",
						title: "The race to reconnect Tonga",
						description:
							"How engineers will repair the undersea communications cable severed by the recent volcanic eruption",
						publication: "Reuters",
						year: 2022,
						thumbnail:
							"https://graphics.reuters.com/TONGA-VOLCANO/znpnejbjovl/cdn/images/reuters-graphics.jpg",
					},
					{
						workSection: "allDigitalWork",
						workFeature: "",
						link: "https://graphics.reuters.com/CHINA-BHUTAN/BORDER/zjvqknaryvx/",
						slug: "Politics",
						title: "China-Bhutan border",
						description: "",
						publication: "Reuters",
						year: 2022,
						thumbnail:
							"https://graphics.reuters.com/CHINA-BHUTAN/BORDER/zjvqknaryvx/cdn/images/reuters-graphics.jpg",
					},
					{
						workSection: "allDigitalWork",
						workFeature: "",
						link: "https://www.reuters.com/investigates/special-report/brazil-environment-military/",
						slug: "Environment",
						title: "Military missteps in the Amazon",
						description:
							"Wrangled QGIS to build a map showing the extent of deforestation and forest fires in Brazil’s Amazon rainforest.",
						publication: "Reuters",
						year: 2021,
						thumbnail:
							"https://aditibhandari.github.io/img/github-repo.webp",
					},
					{
						workSection: "allDigitalWork",
						workFeature: "",
						link: "https://graphics.reuters.com/MYANMAR-POLITICS/DETENTIONS/jbyvrdaznve/index.html",
						slug: "Conflict",
						title: "Myanmar’s new wave of detainees",
						description:
							"Worked with the Myanmar bureau to visualize the number of people detained following the military coup. Also tracked the reported gender, age and cause of death of the <a href='https://graphics.reuters.com/MYANMAR-POLITICS/dgkplekqgvb/myanmar-deaths.jpg' class='sample_text_link' target='_blank' rel='noopener noreferrer'>people killed by security forces</a>.",
						publication: "Reuters",
						year: 2021,
						thumbnail:
							"https://graphics.reuters.com/MYANMAR-POLITICS/DETENTIONS/jbyvrdaznve/img/share.png",
					},
					{
						workSection: "allDigitalWork",
						workFeature: "",
						link: "https://graphics.reuters.com/ARMENIA-AZERBAIJAN/jbyprxxqbpe/index.html",
						slug: "Conflict",
						title: "Nagorno-Karabakh conflict",
						description:
							"Created a scrolly explainer with annotated maps and photos to walk readers through the Nagorno Karabakh conflict and its impact on both local populations and international oil supplies.",
						publication: "Reuters",
						year: 2020,
						thumbnail:
							"https://graphics.reuters.com/ARMENIA-AZERBAIJAN/jbyprxxqbpe/img/share-card.png",
					},
					{
						workSection: "allDigitalWork",
						workFeature: "",
						link: "https://graphics.reuters.com/INDIA-CITIZENSHIP/PROTESTS/jxlbpgqlpqd/index.html",
						slug: "Conflict",
						title: "India's citizenship protests",
						description:
							"Visualized the anti-CAA and pro-CAA demonstrations that took place nearly every day for several months, and calculated the death toll and use of violence.",
						publication: "Reuters",
						year: 2020,
						thumbnail:
							"https://graphics.reuters.com/INDIA-CITIZENSHIP/PROTESTS/jxlbpgqlpqd/images/share-card.png",
					},
					{
						workSection: "allDigitalWork",
						workFeature: "",
						link: "https://graphics.reuters.com/HEALTH-CORONAVIRUS-SCHOOLS/0100B5KQ43K/index.html",
						slug: "COVID",
						title: "COVID-19 School closures",
						description:
							"Built a map, collected data and maintained a tracker of all the national and local school closures. Also available in Spanish.",
						publication: "Reuters",
						year: null,
						thumbnail:
							"https://aditibhandari.github.io/img/github-repo.webp",
					},
					{
						workSection: "allDigitalWork",
						workFeature: "",
						link: "https://www.reuters.com/investigates/special-report/juul-ecigarette/",
						slug: "Health",
						title: "Juul's Nicotine Addiction",
						description:
							"Made charts and illustrations based on research data and scientific patents for a Reuters Special Report on Juul.",
						publication: "Reuters",
						year: null,
						thumbnail:
							"https://aditibhandari.github.io/img/github-repo.webp",
					},
					{
						workSection: "allDigitalWork",
						workFeature: "",
						link: "https://graphics.reuters.com/INDIA-ELECTION-PROMISES/010091DR1ZR/index.html",
						slug: "Politics",
						title: "Modi's Report Card",
						description:
							"Collaborated with a reporter to assess progress on the Indian PM's previous election promises – sometimes with a chart.",
						publication: "Reuters",
						year: null,
						thumbnail:
							"https://aditibhandari.github.io/img/github-repo.webp",
					},
				],
			},
			{
				page: "work",
				section: "printWork",
				title: "print work",
				text: "I also design print graphics, contraints can be fun challenge to design for and around. Over last few years I've owned and co-owned responsibility of our graphics packages for big sporting events like the TDF and the Euros, coordinating with editors and translation teams along with designing and editing graphics.",
				stories: [
					{
						workSection: "allPrintWork",
						workFeature: null,
						link: "https://graphics.reuters.com/MYANMAR-POLITICS/dgkplekqgvb/myanmar-deaths.jpg",
						slug: "Conflict",
						title: "Myanmar protest deaths",
						description: "",
						publication: "Reuters",
						year: null,
						thumbnail:
							"https://aditibhandari.github.io/img/github-repo.webp",
					},
					{
						workSection: "allPrintWork",
						workFeature: null,
						link: "https://graphics.reuters.com/CYCLISME-FRANCE/xegpboozdvq/CYCLISME-FRANCE-ETAPES19-21.jpg",
						slug: "Culture",
						title: "Tour De France",
						description: "",
						publication: "Reuters",
						year: null,
						thumbnail:
							"https://aditibhandari.github.io/img/github-repo.webp",
					},
					{
						workSection: "allPrintWork",
						workFeature: null,
						link: "https://graphics.reuters.com/HEALTH-CORONAVIRUS/nmoparzyeva/africa-vaccine-delivery.jpg",
						slug: "COVID",
						title: "Africa Vaccines",
						description:
							"Built Google Sheets template to help the Reuters Africa bureaus compile and cross-check Africa vaccine delivery data. Designed map and chart of coronavirus vaccine deliveries to Africa through the WHO co-led COVAX program.",
						publication: "Reuters",
						year: null,
						thumbnail:
							"https://aditibhandari.github.io/img/github-repo.webp",
					},
					{
						workSection: "allPrintWork",
						workFeature: null,
						link: "https://graphics.reuters.com/UGANDA-ELECTION/bdwvkygdgvm/uganda-elections-results.jpg",
						slug: "Politics",
						title: "Uganda Elections",
						description:
							"Pitched and made a graphic for the run-up to the 2021 Ugandan election. Highlighted the incumbent and key frontrunner, and visualized the results of the last 5 elections.",
						publication: "Reuters",
						year: null,
						thumbnail:
							"https://aditibhandari.github.io/img/github-repo.webp",
					},
					{
						workSection: "allPrintWork",
						workFeature: null,
						link: "https://graphics.reuters.com/AFRICA-PRESIDENTS/xegpbenrwvq/african-leaders-tenure.jpg",
						slug: "Politics",
						title: "Africa Leader Tenures",
						description:
							"Designed and made a graphic comparing the longest continuous tenures of the African leaders currently in power.",
						publication: "Reuters",
						year: null,
						thumbnail:
							"https://aditibhandari.github.io/img/github-repo.webp",
					},
					{
						workSection: "allPrintWork",
						workFeature: null,
						link: "https://graphics.reuters.com/NICARAGUA-POLITICS/ORTEGA/nmopaddoeva/srep_nicaragua-media.jpg",
						slug: "Politics",
						title: "Ortega Media Holdings",
						description:
							"Traced the family tree Nicaragua's President Ortega for a Reuters investigation into their media empire and business holdings.",
						publication: "Reuters",
						year: null,
						thumbnail:
							"https://aditibhandari.github.io/img/github-repo.webp",
					},
					{
						workSection: "allPrintWork",
						workFeature: null,
						link: "https://graphics.reuters.com/ASIA-STORM/INDIA/jbyprlmynpe/india-cyclone-nisarga.jpg",
						slug: "Climate",
						title: "Cyclone Nisarga",
						description:
							"Mapped and updated the path of cyclone Nisarga – while it passed over my city.",
						publication: "Reuters",
						year: null,
						thumbnail:
							"https://aditibhandari.github.io/img/github-repo.webp",
					},
					{
						workSection: "allPrintWork",
						workFeature: null,
						link: "https://graphics.reuters.com/AUSTRALIA-BUSHFIRES/0100B4VL2PQ/temperature-rainfall-trends.jpg",
						slug: "Climate",
						title: "Australia Drought",
						description:
							"Compared data of Australia's annual average rainfall and temperature with a 30-year baseline average.",
						publication: "Reuters",
						year: null,
						thumbnail:
							"https://aditibhandari.github.io/img/github-repo.webp",
					},
					{
						workSection: "allPrintWork",
						workFeature: null,
						link: "https://graphics.reuters.com/AUSTRALIA-BUSHFIRES/0100B4RE2HB/nsw-air-pollution.jpg",
						slug: "Environment",
						title: "Australia Air Pollution",
						description:
							"Tracked the PM 2.5 levels in Australia's state of New South Wales shortly before and during the 2020 bushfire season.",
						publication: "Reuters",
						year: null,
						thumbnail:
							"https://aditibhandari.github.io/img/github-repo.webp",
					},
				],
			},
			{
				page: "projects",
				section: "resources",
				title: "resources",
				text: "",
				stories: [
					{
						workSection: "resources",
						workFeature: "faveProjects",
						link: "https://github.com/AditiBhandari/south-asia-data-sources",
						slug: null,
						title: "South Asia Data Sources",
						description:
							"Growing list of govermental, research and other sources of data about India and the South Asia subcontinent.",
						publication: null,
						year: null,
						thumbnail:
							"https://aditibhandari.github.io/img/github-repo.webp",
					},
					{
						workSection: "resources",
						workFeature: "faveProjects",
						link: "https://github.com/AditiBhandari/data-journalism-early-career-tips",
						slug: null,
						title: "NICAR 18 Early Career Tips",
						description:
							"A list of community groups and resources for young and early-career data journalists. Made with Madi Alexander for <a class='sample_text_link' href='https://twitter.com/search?q=aditihbhandari%20%23NICAR18&amp;src=typd' target='_blank' rel='noopener noreferrer'>#NICAR18</a>",
						publication: null,
						year: null,
						thumbnail:
							"https://aditibhandari.github.io/img/github-repo.webp",
					},
				],
			},
			{
				page: "projects",
				section: "lightning talks",
				title: "lightning talks",
				text: "",
				stories: [
					{
						workSection: "lightning talk",
						workFeature: "faveProjects",
						link: "https://aditibhandari.github.io/nicar17-slides/",
						slug: null,
						title: "Self-Care For Nerds",
						description:
							"Pitched and gave a lightning talk at #NICAR17 about physical self-care as a developer, journalist, or just someone who sits at a computer all day. Here are my slides and speaker notes.",
						publication: null,
						year: null,
						thumbnail:
							"https://aditibhandari.github.io/img/github-repo.webp",
					},
					{
						workSection: "lightning talk",
						workFeature: "",
						link: "http://slides.com/dittybhandari/learn/fullscreen#/",
						slug: null,
						title: "Journalism + Code",
						description:
							"My friend Eunice and I gave a talk to a freshman multimedia reporting class about why they should learn how to code, using Learn.KnightLab, the tutorial website I worked on.",
						publication: null,
						year: null,
						thumbnail:
							"https://aditibhandari.github.io/img/github-repo.webp",
					},
					{
						workSection: "lightning talk",
						workFeature: "",
						link: "http://slides.com/dittybhandari/deck-8/fullscreen#/",
						slug: null,
						title: "Design Thinking Irl",
						description:
							"The design process sometimes seems like a drag, but it can help you save time and create a well-developed project. And here's the kicker; you're probably already following the process in your daily life.",
						publication: null,
						year: null,
						thumbnail:
							"https://aditibhandari.github.io/img/github-repo.webp",
					},
				],
			},
		],
	};
</script>

<header>
	<Nav />
</header>

<main>
	<section class="homepage intro">
		<p>
			Hi! I'm a data viz developer at <a
				class="intro_link"
				href="http://graphics.reuters.com/"
				target="_blank"
				rel="noopener noreferrer">Reuters</a
			>
			in Bangalore. I'm a newly-minted Brit living in India, and have previously
			worked at the Hindustan Times in India, and at
			<a
				class="intro_link"
				href="https://wamu.org/search/go?q=aditi%20bhandari"
				target="_blank"
				rel="noopener noreferrer">WAMU 88.5</a
			>, NPR,
			<a
				class="intro_link"
				href="https://www.texastribune.org/about/staff/aditi-bhandari/"
				target="_blank"
				rel="noopener noreferrer">The Texas Tribune,</a
			>
			and
			<a
				class="intro_link"
				href="https://slides.com/aditibhandari/spotlight#/15"
				target="_blank"
				rel="noopener noreferrer">The Boston Globe</a
			> in the U.S..
		</p>
	</section>

	{#each sectionList.sections as section}
		<!-- {#if section.page === "home"} -->
		<section class="section_{section.section}">
			{#if section.title}
				<h3>{section.title}</h3>
			{/if}

			{#if section.text}
				<p>{@html section.text}</p>
			{/if}

			{#if section.stories.length > 1}
				<div class="section_samples">
					{#each section.stories as story}
						<article class="sample">
							<a
								class="sample_link"
								href={story.link}
								target="_blank"
								rel="noopener noreferrer"
							>
								{#if story.slug}
									<p class="sample_slug">{story.slug}</p>
								{/if}
								<p class="sample_title">
									<span class="sample_title_border"
										>{story.title}</span
									>
								</p>
								<picture>
									<!-- <source type="image/webp" srcset="img/myanmar-protests.webp">
									<source type="image/jpeg" srcset="img/myanmar-protests.jpg"> -->
									<img
										class="sample_image"
										src={story.thumbnail}
										alt=""
									/>
								</picture>
							</a>
							<section class="sample_desc">
								<p class="sample_text">
									{@html story.description}
								</p>

								{#if story.publication && story.year}
									<p class="sample_skills">
										{story.publication} | {story.year}
									</p>
								{/if}
							</section>
						</article>
					{/each}
				</div>
			{/if}
		</section>
		<!-- {/if} -->
	{/each}
</main>

<style>
	main {
		color: #191919;
		max-width: 1200px;
		margin-left: auto;
		margin-right: auto;
		padding-bottom: 100px;
	}

	section.intro {
		margin-bottom: 40px;
	}

	section.intro > p {
		max-width: 660px;
		font-size: 1em;
		font-weight: 400;
		line-height: 1.75;
		margin: 0px 0px 10px 0px;
	}

	/* WORK SAMPLES */

	.section_samples {
		width: 100%;
		max-width: 1200px;
		margin-left: auto;
		margin-right: auto;
		flex-wrap: wrap;
		display: flex;
		align-content: space-between;
		justify-content: space-between;
	}

	section h3 {
		margin: 0px 10px 10px 0;
		font-size: 1.5em;
		font-family: "Biryani", sans-serif;
		font-style: normal;
		font-weight: 300;
		display: inline-block;
	}

	.sample {
		width: 31%;
		margin-bottom: 40px;
	}

	.sample_link {
		text-decoration: none;
		color: #191919;
	}

	.sample_link:hover .sample_title_border,
	.section_more_link:hover {
		border-bottom: solid 4px #227f7f;
	}

	.sample_link:hover .sample_image {
		opacity: 0.7;
	}

	.sample_slug {
		margin: 0;
		text-transform: uppercase;
		font-family: "Biryani", sans-serif;
		font-style: normal;
		font-weight: 400;
		font-size: 0.875em;
		color: #737373;
	}

	.sample_title {
		margin: 5px 0;
		font-family: "Open Sans", sans-serif;
		font-weight: 600;
		font-size: 1em;
		color: #191919;
	}

	.sample_title_border {
		border-bottom: solid 4px rgba(34, 127, 127, 0);
		transition: border-bottom ease-in-out 0.1s;
	}

	picture {
		margin: 0;
	}

	.sample_image {
		width: 100%;
		max-height: 200px;
		object-fit: cover;
		margin: 0;
		padding-top: 4px;
		opacity: 1;
		position: relative;
		transition: opacity ease-in-out 0.1s;
	}

	.sample_desc {
		width: 100%;
	}

	.sample_text {
		margin: 3px 0 0 0;
		font-size: 0.9em;
		font-family: "Open Sans", sans-serif;
		font-weight: 400;
		line-height: 1.4;
	}

	.sample_skills {
		font-size: 0.8em;
		margin: 3px 0 0 0;
		color: #737373;
		font-weight: 400;
		font-family: "Open Sans", sans-serif;
	}

	.hidden {
		display: none;
	}
</style>
