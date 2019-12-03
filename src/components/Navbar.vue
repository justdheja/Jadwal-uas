<template>
    <div id="navs">
        <nav class="navbar is-primary" role="navigation" aria-label="main navigation">
            <div class="container">
            <div class="navbar-brand">
                <div class="navbar-item">
                    <div class="title">
                        <router-link to="/" class="has-text-white">UAS</router-link> 
                    </div>
                </div>

                <a role="button" class="navbar-burger burger" aria-label="menu" aria-expanded="false" data-target="navbarBasicExample">
                <span aria-hidden="true"></span>
                <span aria-hidden="true"></span>
                <span aria-hidden="true"></span>
                </a>
            </div>

            <div id="navbarBasicExample" class="navbar-menu">
                <div class="navbar-start">
                <a class="navbar-item">
                    <router-link to="/" class="has-text-white">Home</router-link> 
                </a>

                <div class="navbar-item">
                    <router-link to="/about" class="has-text-white">About</router-link> 
                </div>

                </div>

                <div class="navbar-end">
                <div class="navbar-item">
                    
                </div>
                </div>
            </div>
            </div>
            </nav>
    </div>
</template>

<script>
export default {
    name: 'navbar',
}
</script>