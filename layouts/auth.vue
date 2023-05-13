<template>
    <div>
<header>
    <nav>
        <nuxtLink to="/">Home</nuxtLink> 
        <ul>
            <li> <nuxtLink to="/about">About</nuxtLink> </li>
            <li> <nuxtLink to="/products">products</nuxtLink> </li>
        </ul>   
    </nav>
</header>
    </div>
    <div>
        <slot />
    </div>
    <footer>
        <p> &copy; 2023 coi-lance</p>
    </footer>
</template>


<style  scoped>
.router-link-exact-active{
    color: teal;
}


</style>