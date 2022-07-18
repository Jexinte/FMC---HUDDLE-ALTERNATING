<template>
    <section class="welcome">
        <!-- HEADER -->
        <header>
            <nav>
                <div class="logo">
                    <img src="../assets/images/logo.svg" alt="Logo">
                </div>

                <a href="#" id="TryIt">Try It Free</a>
            </nav>
        </header>

    <div class="welcome-description">
            <div class="left">

                <h1 class="main-title">Build The Community Your Fans Will Love</h1>
        
                <p class="main-description">Huddle re-imagines the way we build communities. You have a voice,but so does your audience.Create connections with your users as you engage in genuine discussion. </p>
        
                <a href="#" class="started">Get Started For Free</a>
            </div>
        <div class="right">
            <img src="../assets/images/illustration-mockups.svg" alt="Mockups">

        </div>
    </div>

    </section>
</template>

<style scoped>

@media screen and (min-width:993px) {
         .welcome {
        padding:45px 11px 0;
    background-image: url('../assets/images/bg-hero-desktop.svg');
      background-color:var(--veryPaleCyan);
      /* background-size: cover; */
}



header{
    margin-bottom: 4em;
    padding-inline: 2em;
}
header nav {
    display: flex;
    justify-content: space-between;
}

header #TryIt {
    color:var(--veryDarkCyan);
    font-family: var(--openSans);
    font-weight: var(--700);
    background-color: white;
    border-radius: 20px;
    padding-inline: 28px;
    padding-block: 9px;
    position: relative;
    bottom: 8px;
    box-shadow: 5px 5px 10px rgba(0,0,0,0.2);
}

header #TryIt:hover{
    color:var(--grayishBlue)
}
.logo img {
    height: 22px;
}
.welcome-description {
max-width: 100%;
display: flex;
text-align: center;
padding-bottom: 47px;
padding-inline: 2em;
gap:1em;
}

.left{
    display: flex;
    flex-direction: column;
    gap: 2em;
    text-align: left;
}

.welcome-description h1 {
    font-family: var(--poppins);
    font-weight: var(--600);
    font-size: 1.5em;
    width: 63%;
}

.welcome-description img {
    width: 100%;
}

.main-description {
    font-family: var(--openSans);
    font-size: 17px;
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
}

}

/* MOBILE */

@media screen and (max-width:992px) {

    .welcome {
        padding:45px 11px 0;
    background-image: url('../assets/images/bg-hero-desktop.svg');
      background-color:var(--veryPaleCyan);
      /* background-size: cover; */
}

.welcome-description h1 {
    font-family: var(--poppins);
    font-weight: var(--600);
    font-size: 1.5em;
}
header{
    margin-bottom: 4em;
}
header nav {
    display: flex;
    justify-content: space-between;
}

header #TryIt {
    color:var(--veryDarkCyan);
    font-family: var(--openSans);
    font-weight: var(--700);
    background-color: white;
    border-radius: 20px;
    padding-inline: 28px;
    padding-block: 9px;
    position: relative;
    bottom: 8px;
    box-shadow: 5px 5px 10px rgba(0,0,0,0.2);
}

header #TryIt:hover{
    color:var(--grayishBlue)
}
.logo img {
    height: 22px;
}
.welcome-description {
max-width: 100%;
display: flex;
flex-direction: column;
gap: 2em;
text-align: center;
padding-bottom: 47px;
}

.welcome-description img {
    width: 100%;
}

.main-description {
    font-family: var(--openSans);
    font-size: 17px;
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
}



    }
</style>