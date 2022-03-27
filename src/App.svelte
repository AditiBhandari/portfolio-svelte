<script>
	import Nav from './components/Nav.svelte';
	import StoryCard from './components/StoryCard.svelte';

	let sectionList = {
		sections: [
			{
				page: "home",
				section: "work",
				title: "my favourite work",
				text: "",
				stories: [
					{
						"link": "https://graphics.reuters.com/PARALYMPICS-2022/EQUIPMENT/dwpkrlmnrvm/",
						"slug": "Culture",
						"title": "Built to win",
						"description": "The adaptive sports tools powering the 2022 Winter Paralympics.",
						"publication": "Reuters",
						"year": 2022,
						"thumbnail": "https://graphics.reuters.com/PARALYMPICS-2022/EQUIPMENT/dwpkrlmnrvm/cdn/images/reuters-graphics.jpg"
					},
					{
						"link": "https://graphics.reuters.com/GLOBAL-RACE/BTS-FANS/nmopajgmxva/",
						"slug": "Culture",
						"title": "BTS ARMY's fundraising power",
						"description": "Interviewed BTS fans and experts, created the data graphics and designed and built the page. It won an Award of Excellence at the SND: Best of Digital News Design awards, and BTS fans showed their love on Twitter.",
						"publication": "Reuters",
						"year": 2020,
						"thumbnail": "https://graphics.reuters.com/GLOBAL-RACE/BTS-FANS/nmopajgmxva/img/share-card.png"
					},
					{
						"link": "https://graphics.reuters.com/MYANMAR-POLITICS/zjpqkkoaqpx/",
						"slug": "Conflict",
						"title": "Myanmar protest deaths",
						"description": "The tragedy still unfolding in Myanmar, told through the profiles of seven people who died after the military cracked down on protests after the 2021 coup.",
						"publication": "Reuters",
						"year": 2021,
						"thumbnail": "https://graphics.reuters.com/MYANMAR-POLITICS/zjpqkkoaqpx/img/share.png"
					}
				]
			},
			{
				page: "home",
				section: "projects",
				title: "my favourite projects",
				text: "",
				stories: []
			},
			{
				page: "work",
				section: "originalReporting",
				title: "original reporting",
				text: "List the awards won",
				stories: []
			},
			{
				page: "work",
				section: "longTermCoverage",
				title: "long-term coverage",
				text: "List the awards won",
				stories: []
			},
			{
				page: "work",
				section: "digitalWork",
				title: "more digital work",
				text: "I design page and/or work on graphics depending on the project. Always looking for opportunities to templatise work and document for future use. Lately been making a more concerted effort to make projects accessible while covering, and wrapping it into documentation and training",
				stories: []
			},
			{
				page: "work",
				section: "printWork",
				title: "more print work",
				text: "I also design print graphics, contraints can be fun challenge to design for and around. Over last few years I've owned and co-owned responsibility of our graphics packages for big sporting events like the TDF and the Euros, coordinating with editors and translation teams along with designing and editing graphics.",
				stories: []
			},
			{
				page: "projects",
				section: "resources",
				title: "resources",
				text: "",
				stories: []
			},
			{
				page: "projects",
				section: "lightning talks",
				title: "lightning talks",
				text: "",
				stories: []
			},
			{
				page: "projects",
				section: "tutorials",
				title: "tutorials",
				text: "",
				stories: []
			},
		],
	};

	let storyList = {
		stories: [
			{
				"link": "https://graphics.reuters.com/PARALYMPICS-2022/EQUIPMENT/dwpkrlmnrvm/",
				"slug": "Culture",
				"title": "Built to win",
				"description": "The adaptive sports tools powering the 2022 Winter Paralympics.",
				"publication": "Reuters",
				"year": 2022,
				"thumbnail": "https://graphics.reuters.com/PARALYMPICS-2022/EQUIPMENT/dwpkrlmnrvm/cdn/images/reuters-graphics.jpg"
			},
			{
				"link": "https://graphics.reuters.com/GLOBAL-RACE/BTS-FANS/nmopajgmxva/",
				"slug": "Culture",
				"title": "BTS ARMY's fundraising power",
				"description": "Interviewed BTS fans and experts, created the data graphics and designed and built the page. It won an Award of Excellence at the SND: Best of Digital News Design awards, and BTS fans showed their love on Twitter.",
				"publication": "Reuters",
				"year": 2020,
				"thumbnail": "https://graphics.reuters.com/GLOBAL-RACE/BTS-FANS/nmopajgmxva/img/share-card.png"
			},
			{
				"link": "https://graphics.reuters.com/MYANMAR-POLITICS/zjpqkkoaqpx/",
				"slug": "Conflict",
				"title": "Myanmar protest deaths",
				"description": "The tragedy still unfolding in Myanmar, told through the profiles of seven people who died after the military cracked down on protests after the 2021 coup.",
				"publication": "Reuters",
				"year": 2021,
				"thumbnail": "https://graphics.reuters.com/MYANMAR-POLITICS/zjpqkkoaqpx/img/share.png"
			}
		]
	};
</script>

<header>
	<Nav />
</header>


<main>
	<section class="homepage intro">
		<p>Hi! I'm a data viz developer at <a class='intro_link' href='http://graphics.reuters.com/' target='_blank' rel='noopener noreferrer'>Reuters</a> in Bangalore. I'm a newly-minted Brit living in India, and have previously worked at the Hindustan Times in India, and at <a class='intro_link' href='https://wamu.org/search/go?q=aditi%20bhandari' target='_blank' rel='noopener noreferrer'>WAMU 88.5</a>, NPR, <a class='intro_link' href='https://www.texastribune.org/about/staff/aditi-bhandari/' target='_blank' rel='noopener noreferrer'>The Texas Tribune,</a> and <a class='intro_link' href='https://slides.com/aditibhandari/spotlight#/15' target='_blank' rel='noopener noreferrer'>The Boston Globe</a> in the U.S..</p>
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
					{#each storyList.stories as story}

						<article class="sample">
							<a class="sample_link" href="{story.link}" target="_blank" rel="noopener noreferrer">
								{#if story.slug}
									<p class="sample_slug">{story.slug}</p>
								{/if}
								<p class="sample_title"><span class="sample_title_border">{story.title}</span></p>
								<picture>
									<!-- <source type="image/webp" srcset="img/myanmar-protests.webp">
									<source type="image/jpeg" srcset="img/myanmar-protests.jpg"> -->
									<img class="sample_image" src="{story.thumbnail}" alt="">
								</picture>
							</a>
							<section class="sample_desc">
								<p class="sample_text">{@html story.description}</p>
								<p class="sample_skills">{story.publication} | {story.year}</p>
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
		margin-top: 20px;
		flex-wrap: wrap;
		display: flex;
		align-content: space-between;
	}

	.sample {
		width: 31%;
		min-width: 250px;
		max-width: 330px;
		margin-right: 3%;
		margin-bottom: 40px;
		flex-grow: 1;
		flex-shrink: 1;
		flex-basis: 0;
	}

	.sample_link {
		text-decoration: none;
		color: #191919;
	}

	.sample_link:hover .sample_title_border, .section_more_link:hover {
		border-bottom: solid 4px #227f7f; 
	}

	.sample_link:hover .sample_image { opacity: 0.7; }

	.sample_slug {
		margin: 0;
		text-transform: uppercase;
		font-family: 'Open Sans', sans-serif;
		font-style: normal;
		font-weight: 400;
		font-size: 0.875em;
		color: #737373;
	}

	.sample_title {
		margin: 5px 0;
		font-family: 'Open Sans', sans-serif;
		font-weight: 700;
		font-size: 1em;
		color: #191919;
	}

	.sample_title_border {
		border-bottom: solid 4px #fff;
		transition: border-bottom ease-in-out 0.1s;
	}

	picture { margin: 0; }

	.sample_image {
		width: 100%;
		margin: 0;
		padding-top: 4px;
		opacity: 1;
		position: relative;
		transition: opacity ease-in-out 0.1s;
	}

	.sample_desc { width: 100%; }

	.sample_text {
		margin: 3px 0 0 0;
		font-size: 0.9em;
		font-family: 'Open Sans', sans-serif;
		font-weight: 400;
		line-height: 1.4;
	}

	.sample_text_link {
		font-weight: 600;
		color: inherit;
		text-decoration: none;
		border-bottom: solid 2px #227f7f;
		transition: border-bottom ease-in-out 0.1s;
	}

	.sample_text_link:hover { border-bottom: solid 4px #227f7f; }

	.sample_skills {
		font-size: 0.8em;
		margin: 3px 0 0 0;
		color: #737373;
		font-weight: 400;
		font-family: 'Open Sans', sans-serif;
	}

	.hidden { display: none; }



</style>