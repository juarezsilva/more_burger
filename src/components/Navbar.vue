<template>
    <div id="nav">
        <router-link to="/" id="logo-url">
            <img :src="logo" :alt="alt" id="logo">
        </router-link>
        <router-link to="/" id="flash">Home</router-link>
        <router-link to="/pedidos" id="flash">Pedidos</router-link>
    </div>
</template>

<script>
export default {
    name: 'Navbar',
    props: ["logo", "alt"]
}
</script>

<style scoped>
    #nav {
        background-color: #222;
        border-bottom: 4px;
        padding: 15px 50px;
        display: flex;
        justify-content: flex-end;
        align-items: center;
    }

    #nav #logo-url {
        margin: auto;
        margin-left: 0;
    }

    #logo {
        width: 40px;
        height: 40px;
    }

    #flash {
        background-color: #222;
        padding: 10px;
        border-radius: 5px;
    }

    #flash:hover {
        background-color: #333;         
    }

    #nav a {
        color: #FCBA03;
        text-decoration: none;
        font-size: 18px;
        margin: 12px;        
        transition: .5s;
    }

    #nav a:hover {
        color: cyan;
    }

</style>