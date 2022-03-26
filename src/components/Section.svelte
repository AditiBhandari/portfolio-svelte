<script>
	export let sectionTitle;
	import StoryCard from './StoryCard.svelte';

	let stories = [
		{
			"section": "online",
			"link": "https://graphics.reuters.com/CHINA-CRASH/znvneqennpl/index.html",
			"slug": "Breaking news",
			"title": "Plane crash in China",
			"description": "A China Eastern Airlines passenger jet with 132 people on board crashed in the mountains of southern China en route from the southwestern city of Kunming to Guangzhou, on the east coast.",
			"skills": "HTML/CSS/JS, ai2html/Illustrator",
			"publication": "Reuters",
			"date": "March 22, 2022",
			"year": 2022,
			"thumbnail": "https://graphics.reuters.com/CHINA-CRASH/znvneqennpl/cdn/images/reuters-graphics.jpg"
		},
		{
			"section": "online",
			"link": "https://graphics.reuters.com/PARALYMPICS-2022/EQUIPMENT/dwpkrlmnrvm/",
			"slug": "Culture",
			"title": "Built to win",
			"description": "The adaptive sports tools powering the 2022 Winter Paralympics",
			"skills": "HTML/CSS/JS, ai2html/Illustrator",
			"publication": "Reuters",
			"date": "March 11, 2022",
			"year": 2022,
			"thumbnail": "https://graphics.reuters.com/PARALYMPICS-2022/EQUIPMENT/dwpkrlmnrvm/cdn/images/reuters-graphics.jpg"
		}
	];
</script>

<section>
	<h2>{sectionTitle}</h2>
	{#each stories as {slug, title, link, description, skills, publication, date, thumbnail}}
		<StoryCard slug={slug} title={title} link={link} description={description} skills={skills} publication={publication} date={date} thumbnail={thumbnail}></StoryCard>
	{/each}
</section>