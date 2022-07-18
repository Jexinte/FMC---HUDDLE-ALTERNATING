<template>
<section class="offers">
<div class="services">
    <div class="box growth">
        <div class="left">

            <h2 v-for="data in offersData">{{data['box1'].title1}}</h2>
            <p v-for="data in offersData">{{data['box1'].text1}}</p>
        </div>
        <div class="right">
            <img src="@/assets/images/illustration-grow-together.svg" alt="People watching">
        </div>


    </div>

    <div class="box flowing">
        <div class="left-flowing">            
            <img src="@/assets/images/illustration-flowing-conversation.svg" alt="People speaking around table">
        </div>
        <div class="right-flowing">

            <h2 v-for="data in offersData">{{data['box2'].title2}}</h2>
            <p v-for="data in offersData">{{data['box2'].text2}}</p>
        </div>

    </div>
    <div class="box growth">
        <div class="left">
            
            <h2 v-for="data in offersData">{{data['box3'].title3}}</h2>
        <p v-for="data in offersData">{{data['box3'].text3}}</p>
            </div>
            <div class="right">
    
                <img src="@/assets/images/illustration-your-users.svg" alt="People with text illustrations">
                </div>

    </div>

    <div class="communityBuild">
    <h2>Ready To Build Your Community?</h2>
    <a href="#" class="started">Get Started For Free</a>
</div>
</div>

</section>
</template>

<script>
export default {
    
 data(){
    return {
        offersData : [
            {
                box1: {
                    title1 : 'Grow Together',
                    text1 : `Generate meaningful discussions with your audience and build a strong, loyal community. Think of the insightful conversations you miss out on with a feedback form.`
                },

                box2: {
                    title2 : 'Flowing Conversations',
                    text2 : `You wouldn't paginate a conversation in real life, so why do it online ? our threads have just-in-time loading for a more natural flow.`
                },

                box3: {
                    title3 : 'Your Users',
                    text3 : `It takes no time at all to integrate Huddle with your app's authentication solution. This means, once signed in to your app, your users can start chatting immediately.`
                }
            }
        ]
    }
 },


}
</script>
<style scoped>
.started:hover{
    opacity: .5;
}

.box{
    box-shadow: 0px 1px 10px rgba(0,0,0,0.1);
    border-radius: 10px;
}

@media screen and (min-width:993px){
.offers {
margin-top: 117px;
padding-inline: 2em;
}

.services {
display: flex;
flex-direction: column;
gap:2em;
}
.box {
max-width: 100%;
text-align: center;
display: flex;
gap: 4em;
padding-inline: 0.8em;
padding-block: 3em;

}

.box h2 {
font-family: var(--poppins);
font-weight: var(--600);
}

.box p {
font-family: var(--openSans);
font-weight: var(--400);
color:var(--grayishBlue)
}

.box img {
width: 100%;
}

.communityBuild {
background-color: white;
position: relative;
z-index: 5;
display: flex;
flex-direction: column;
align-items: center;
border-radius: 10px;
bottom: -4em;
padding-inline: 1em;
padding-top: 3.5em;
gap: 1.5em;
padding-bottom: 3em;
box-shadow: 5px 5px 10px rgba(0,0,0,0.1);
width: 70%;
margin:  0 auto;
}

.communityBuild h2 {
text-align: center;
color:var(--veryDarkCyan)
}
.started:visited {
color:white;
}
.started {
background-color: var(--pink);
color:white;
font-weight: var(--600);
font-family: var(--openSans);
border-radius: 28px;
padding-top: 14px;
padding-bottom: 14px;
width: 100%;
text-align: center;
}


.growth .left{
display: flex;
flex-direction: column;
justify-content: center;
gap: 1em;
text-align: left;
padding-left: 1em;
}

.flowing .right-flowing {
display: flex;
flex-direction: column;
gap:1em;
justify-content: center;
text-align: left;
}

.communityBuild {
background-color: white;
position: relative;
z-index: 5;
display: flex;
flex-direction: column;
align-items: center;
border-radius: 20px;
bottom: -4em;
padding-inline: 1em;
padding-top: 3.5em;
gap: 1.5em;
padding-bottom: 3em;
box-shadow: 5px 5px 10px rgba(0,0,0,0.1);
}

.communityBuild h2 {
text-align: center;
color:var(--veryDarkCyan);
font-family: var(--poppins);
}
.started:visited {
color:white;
}
.started {
background-color: var(--pink);
color:white;
font-weight: var(--600);
font-family: var(--openSans);
border-radius: 28px;
padding-top: 14px;
padding-bottom: 14px;
width: 100%;
text-align: center;
}

}




/* MOBILE */
@media screen and (max-width:992px) {

.offers {
margin-top: 117px;
padding-inline: 2em;
}

.services {
display: flex;
flex-direction: column;
gap:2em;
}
.box {
max-width: 100%;
text-align: center;
display: flex;
flex-direction: column;
gap: 2em;
padding-inline: 0.8em;
padding-block: 3em;

}

.box h2 {
font-family: var(--poppins);
font-weight: var(--600);
}

.box p {
font-family: var(--openSans);
font-weight: var(--400);
color:var(--grayishBlue)
}

.box img {
width: 100%;
}

.communityBuild {
background-color: white;
position: relative;
z-index: 5;
display: flex;
flex-direction: column;
align-items: center;
border-radius: 20px;
bottom: -4em;
padding-inline: 1em;
padding-top: 3.5em;
gap: 1.5em;
padding-bottom: 3em;
box-shadow: 5px 5px 10px rgba(0,0,0,0.1);
}

.communityBuild h2 {
text-align: center;
color:var(--veryDarkCyan);
font-family: var(--poppins);
}
.started:visited {
color:white;
}
.started {
background-color: var(--pink);
color:white;
font-weight: var(--600);
font-family: var(--openSans);
border-radius: 28px;
padding-top: 14px;
padding-bottom: 14px;
width: 100%;
text-align: center;
}

.growth{
gap:3em;
}
.growth .right {
order: -1;
}

.growth .left{
display: flex;
flex-direction: column;
gap: 1em;
}

.flowing{
gap: 3em;
}

.flowing .right-flowing {
display: flex;
flex-direction: column;
gap:1em;
}
    }
</style>