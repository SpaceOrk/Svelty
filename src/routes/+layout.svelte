<nav>
    <div class="nav-container">
        <a href="/" class="nav-logo" title="Back to Homepage">Page</a>
        <div class="nav-links">
            {#each nav as link}
                {#if link.isShow}
                   <a href={link.href} class="link">{link.title}</a>
                {/if}
            {/each}
        </div>
    </div>
</nav>
<div class="container">
    <slot></slot>
</div>

<style>
    .container{
        max-width: 1400px;
        margin: 50px auto;
    }
</style>
<script>
    const nav = [
        {
            title:"About me",
            href:"/about",
            isShow: true
        },
        {
            title:"Blog",
            href:"/blog",
            isShow: true
        },
        {
            title:"My project",
            href:"project",
            isShow: true
        },
        {
            title:"contact",
            href:"contact",
            isShow: true
        },
        {
            title:"temp",
            href:"temp",
            isShow: false
        }
    ]
</script>