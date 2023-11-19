<div class="container">
    <a href="/blog">Go back to blog</a>
    <slot></slot>
</div>
<style>
    .container{
        margin: 50px auto;
        max-width: 800px;
        padding: 0 20px;
    }
    .container a{
        color: rgb(0, 0, 0);
        border: 2px solid black;
    }
</style>