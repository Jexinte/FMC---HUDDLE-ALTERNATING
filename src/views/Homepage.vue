<template>
<WelcomeSection/>
<Offers/>
<Footer/>

</template>

<script>
// @ is an alias to /src

import WelcomeSection from '@/components/WelcomeSection.vue'
import Offers from '@/components/Offers.vue'
import Footer from '@/components/Footer.vue'


export default {
    components : {
    WelcomeSection,
    Offers,
    Footer,
}
}

</script>   

<style>                 

/* Poppins Semi-Bold 600  */
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@600&display=swap');

/* Open Sans Regular 400 / Bold 700 */
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;700&display=swap');
    
:root {
    
    /*  Primary */

        --pink: hsl(322, 100%, 66%);

    /*  Neutral */

        --veryPaleCyan: hsl(193, 100%, 96%);
        --veryDarkCyan: hsl(192, 100%, 9%);
        --grayishBlue: hsl(208, 11%, 55%);

    /* Fonts */
        --18px : 18px;
        --poppins : 'Poppins';
        --openSans : 'Open Sans';
        --400 : 400;
        --600 : 600;
        --700 : 700;
}

*{
        margin:0;
        padding:0;
        box-sizing: border-box;
        text-decoration: none;
        list-style-type: none;
    }

body{
    font-size: var(--18px);
}

</style>
