<script>
    const apps = [
        {
            name: "School Work",
            href: "#" // Make sure to change this after `School Work` page is completed.
        }
    ]
</script>

<style>
    #content-title {
        text-transform: uppercase;
        font-size: 1.25em;
    }

    #app-list a {
        color: inherit;
        text-decoration: none;
    }
</style>

<span id="content-title">Applications</span>
<ul id="app-list">
    {#each apps as {name, href}}
        <li>
            <a href={href}>{name}</a>
        </li>
    {/each}
</ul>
