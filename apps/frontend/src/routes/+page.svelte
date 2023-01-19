<script>
	import discord_profiles from '$lib/images/swabbies.png';
	import tbow_item from '$lib/images/tbow-item.png';
	import team_1 from '$lib/images/wanted.png';
</script>

<svelte:head>
	<title>Competition Standings</title>
	<meta name="description" content="Sith Leaderboard App" />
</svelte:head>

<div class="container mx-auto max-w-[900px]">
	<div class="py-5">
		<div class="bg-green-400 p-5">
			<h1 class="text-white text-left uppercase">Sith</h1>
			<h3 class="text-white">Competition Standings</h3>
		</div>
		<div class="bg-green-400 p-5 my-5 columns-2">
			<h3 class="text-white text-center bg-green-700 py-2 rounded-lg">Competition Standings</h3>
			<h3 class="text-white text-center bg-green-700 py-2 rounded-lg">Activity Log</h3>
		</div>
		<div class="bg-red-700 p-5 my-5" id="team-1">
			<div class="grid grid-cols-12">
				<div class="col-start-0 col-span-2">
					<img class="" src={team_1} alt="team-1">
				</div>
				<div class="col-start-3 col-span-6">
					<h2 class="text-white py-2">Team Name</h2>
					<img src={discord_profiles} alt="discord-team">
				</div>
				<div class="col-start-10 col-span-3">
					<h1 class="text-white text-right py-2">Team Points</h1>
					<h4 class="text-white text-right py-2">Points</h4>
					<h4 class="text-white text-right py-2">Raids Remaining</h4>
				</div>
			</div>
			<div class="grid grid-cols-12">
				<h2 class="col-start-0 col-span-12 text-white px-4 py-2">Most Recent Drop</h2>
			</div>
			<div class="grid grid-cols-12 bg-red-900 p-5 rounded-xl">
				<div class="col-start-0 col-span-2 my-auto">
					<img class="" src={tbow_item} alt="team-1">
				</div>
				<div class="col-start-3 col-span-6">
					<h2 class="text-white py-2">Drop Name</h2>
					<h2 class="text-white py-2">Time Since</h2>
				</div>
				<div class="col-start-10 col-span-3">
					<h2 class="text-white text-right py-2">Points Added</h2>
				</div>
			</div>
		</div>
	</div>
</div>