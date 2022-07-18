<template>


<footer>
    
  
    <div class="main-box">

        <div class="box" >
            <img src="@/assets/images/logo-copie.svg" id="logo" alt="Logo">
    </div>
    <div class="box">
        <img src="@/assets/images/icon-location.svg" class="icon-logo" alt="Pin Location icon">
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua</p>
    </div>
    <div class="box">
        <img src="@/assets/images/icon-phone.svg" class="icon-logo" alt="A phone icon">
        <p>+1-543-123-4567</p>
    </div>
    <div class="box">
        <img src="@/assets/images/icon-email.svg" class="icon-logo" alt="Mail icon">
        <p>example@fylo.com</p>
    </div>

        </div>
    <ul class="firstList">
        <li v-for="lidata in listData">{{lidata}}</li>
    </ul>

    <ul class="secondList">
        <li v-for="lidata2 in listData2">{{lidata2}}</li>
    </ul>

    <div class="medias-copyright">

            <div class="social-medias">
                <font-awesome-icon icon="fa-brands fa-facebook-f" class="fa-brands" id="facebook" />
        <font-awesome-icon icon="fa-brands fa-twitter" class="fa-brands" />
        <font-awesome-icon icon="fa-brands fa-instagram" class="fa-brands" />
        
        </div>

        <div class="copyright">
            <p>© Copyright 2018 Huddle. All rights reserved.</p>
            
        </div>
        
        </div>
</footer>
</template>


<script>

    export default {
        name : 'list',
        data() {
            return {
                listData : ['About Us','What We Do','FAQ'],
                listData2 : ['Career','Blog','Contact Us']
            }
        }
    }
</script>
<style scoped>


.fa-brands:hover{
color : var(--pink);
border: 1px solid var(--pink);
}
body{
    overflow-x: hidden;
}

ul li:hover{
    text-decoration: underline;
}
@media screen and (min-width:993px){


footer {

background-color: var(--veryDarkCyan);
display: flex;
gap:2em;
padding-inline: 1em;
font-family: var(--openSans);
font-weight: var(--400);
color:white;
padding-top: 12em;
padding-bottom:9em;
padding-inline:2em;
}

.medias-copyright {
display: flex;
flex-direction: column;
gap:4em;
justify-content: center;
position: relative;
top:2em;
}
.main-box{
display: flex;
flex-direction: column;
gap:1.5em;
}
ul{
width: 50%;
display: flex;
flex-direction: column;
justify-content: center;
}
.box {
display: flex;
gap: 1em;
white-space: pre-line;
}

#logo {
height: 190px;
}

.icon-logo {
height: 20px;
}
.box:nth-child(2){
position: relative;
bottom: 69px;
white-space: pre-line;
width: 82%;
}

.box:nth-child(3){
position: relative;
bottom: 70px;
}
.box:nth-child(4){
position: relative;
bottom: 52px;
}

.firstList{
display: flex;
flex-direction: column;
gap:1.2em;
cursor: pointer;
margin-bottom: 2em;
}

.secondList{
display: flex;
flex-direction: column;
gap:1.2em;
cursor: pointer;
margin-bottom: 2em;
}



.social-medias {
display: flex;
justify-content: center;
gap:1em;
position: relative;
bottom:1em;
}

.fa-brands {
border: 1px solid white;
border-radius: 50px;
padding:.8em;
cursor: pointer;
}


#facebook {
padding: .8em 1em;
}

.copyright {
text-align: center;
padding-bottom: 3.5em;
position: relative;
top:12em;
}

.copyright p {
white-space: pre;
}

    }






/* MOBILE  */
@media screen and (max-width:992px) {

.main-box{
display: flex;
flex-direction: column;
gap:1.5em;
}

.firstList {
    margin-bottom: 0;
}
footer {

background-color: var(--veryDarkCyan);
display: flex;
flex-direction: column;
gap:2em;
padding-inline: 1em;
font-family: var(--openSans);
font-weight: var(--400);
color:white;
padding-top: 5em;
}


.box {
display: flex;
gap: 1em;

}

#logo {
height: 190px;
}

.icon-logo {
height: 20px;
}
.box:nth-child(2){
position: relative;
bottom: 69px;
}

.box:nth-child(3){
position: relative;
bottom: 70px;
}
.box:nth-child(4){
position: relative;
bottom: 52px;
}

ul{
display: flex;
flex-direction: column;
gap:1.2em;
cursor: pointer;
margin-bottom: 2em;
}

.social-medias {
display: flex;
justify-content: center;
gap:1em;
margin-bottom: 2em;
}

.fa-brands {
border: 1px solid white;
border-radius: 50px;
padding:.8em;
cursor: pointer;
}


#facebook {
padding: .8em 1em;
}

.copyright {
text-align: center;
padding-bottom: 3.5em;
}

    }
</style>