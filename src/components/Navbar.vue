<template>
    <div id="nav">
        <router-link to="/" id="logo-url">
            <img :src="logo" :alt="alt" id="logo">
        </router-link>      
        <Router-Link to="/">Home </Router-Link> 
        <Router-Link to="/pedidos">Pedidos</Router-Link>      
    </div>
</template>

<script>
export default {
    name: "Navbar",
    props: ["logo", "alt"]
}
</script>

<style scoped>
    #nav {
        background-color: #222;
        border-bottom: 4px solid #111;
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
    #nav a {
        color: #FCBA03;
        text-decoration: blue;
        margin: 12px;
        transition: .5s;
    }

    #nav a:hover {
        color: aliceblue;
    }
</style>