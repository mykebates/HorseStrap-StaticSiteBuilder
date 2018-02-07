<template>
    <div id="nuxt_wrapper">
        <div style="display: flex; align-items: center; justify-content: center; height: 100vh;">
            <audio src="/horse.mp3" autoplay></audio>
            <img src="/images/horse.jpg" alt="HorseStrap">
            <h1 style="font-weight: normal;">HorseStrap is now e<span style="font-weight: bold;">neigh</span>bled.</h1>
        </div>
    </div>
</template>

<script>
//import axios from 'axios';
export default {
    asyncData (context) {
        // return axios.get('https://quipvid.com/api/quips')
        // .then((res) => {
        //     console.log(res.data)
        //     return {
        //         name: 'World',
        //         quips: res.data
        //     }
        // });

        return { name: 'HorseStrap' }
    },

    head: {
        title: "Horse'n Around",
        bodyAttrs: {
            class: 'home'
        },
        htmlAttrs: {
            class: ''
        },
    }
}
</script>
