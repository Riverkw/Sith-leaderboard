<script>
async fucntion getName() {
    const name = await fetch('http://localhost:3000')
    return name.json()
}
const promise = getName();
</script>
<h1>hello world</h1>
{#await promise}
<p>Loading...</p>
{:then name}
{name}

{/await}