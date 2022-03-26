<script>
	export let slug;
	export let title;
	export let link;
	export let description;
	export let skills;
	export let publication;
	export let date;
	export let year;
	export let thumbnail;
</script>

<!-- ADD A BUNCH OF NAMED SLOTS HERE WITH FALLBACK -->

<article>
	<p>{slug}</p>
	<img src="{thumbnail}" alt="">
	<h3><a href="{link}" target="_blank">{title}</a></h3>
	<p>{description}</p>
	<p>{skills}</p>
	<p>{publication} | {date}</p>
</article>

<style>
	article {
		background-color: pink;
	}

	img {
		width: 200px;
		height: auto;
	}
</style>