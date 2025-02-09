<template>
    <div>
        <Navbar/>
        <LeftMenuVue/>
        <h1>{{ txt }}</h1>
    </div>
</template>

<script>

    import Navbar from './Navbar.vue';
    import LeftMenuVue from './LeftMenu.vue';


    export default{
        data() {
            return {
                txt : "Main Page"
            }
        },

        methods: {
            
        },

        components: {
            Navbar,
            LeftMenuVue
        }
    }
</script>