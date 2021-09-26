<nav class="navbar">
    <a href="/">Home</a>
    <a href="/about">About</a>
    <a href="/blog">Blog</a>
</nav>

<slot></slot>

<style>
    .navbar{
        display: flex;
        justify-content: space-around;
        align-items: center;
        background-color: aquamarine;
        padding: 2.5em;
        border-radius: 0.5em;
    }
    a{
        transition: all 0.5s ease ;
    }
</style>