<script>
// import { ref, onMounted, onUnmounted } from 'vue'
// export default {
//     setup() {
//         const background = ref(null)
//         const first = ref(null)
//         return {
//             // foreground,
//             background,
//             first,
//         }
//     },
// }
// onMounted(() => {
//     document.addEventListener('scroll', handleScroll)
// })
// onUnmounted(() => {
//     document.removeEventListener('scroll', handleScroll)
// })

// const handleScroll = (evt) => {
//   const scrollY = window.scrollY
//   // decreases as user scrolls
//   first.value.style.opacity =
//     (100 - (scrollY + window.innerHeight - first.value.offsetHeight)) / 100
//   // increases as user scrolls
//   const maxBackgroundSize = 120
//   const backgroundSize = scrollY / (maxBackgroundSize - 100) // increases as user scrolls
//   // zoom the background at a slower rate
//   background.value.style.transform =
//     'scale(' + (100 + backgroundSize * 0.4) / 100 + ')'
// }
</script>


<template>
    <div class="main">
        <link href="https://fonts.googleapis.com/css2?family=Abril+Fatface&
        family=Dancing+Script:wght@600&
        family=Lemonada:wght@600&
        family=Roboto+Mono:wght@200;500&display=swap" rel="stylesheet"></link>
        <link href="https://fonts.googleapis.com/css2?family=Nunito:wght@300;1000&display=swap" rel="stylesheet"></link>

        <div class="navbar">
            <div class="navbaritems">
                <div class="navleft">
                    <a href="#about" class="link-about"><img src="CLlogotrans.png" id="navbarlogo" alt="logo" />
                        <div class="navbarname">CHRISTINE LI</div>
                    </a>
                </div>
                <ul class="navtabs">
                    <li><a href="ChristineLi_Resume.pdf" target="_blank">RESUME</a></li>
                    <!-- <li><a href="#about" class="link-aboutme">ABOUT</a></li> -->
                    <!-- <li><a href="#education" class="link-education">EDUCATION</a></li>
                            <li><a href="#experiences" class="link-experiences">EXPERIENCES</a></li>
                            <li><a href="#projects" class="link-projects">PROJECTS</a></li> -->
                    <li><a href="#dance" class="link-dance">DANCE</a></li>
                    <li><a href="#random" class="link-random">RANDOM</a></li>
                    <li><a href="#contact" class="link-contact">CONTACT</a></li>
                </ul>
            </div>
            <div class="navdividerline"></div>
        </div>
        <section class="landing">
            <!-- <img class="mainimg" ref="background" src="crbhamiltonsteps.jpg"> -->
            <div class="hello" ref="first">
                <h1>Hello! I am Christine Li.</h1>
            </div>
            <!-- <div class="section blurb" ref="second">
                <div>
                    <h2>Learner. Dancer. Researcher.</h2>
                    <p>I'm an undergrad at Columbia University in NYC studying computer science and linguistics. I am from San Francisco Bay Area and Shanghai. I love traveling, reading, dancing, and cooking.
                    </p>      
                </div>
            </div> -->
            <!-- <div class="intro">
                <div class="introleft">
                    <h1 class="greeting">Hello!</h1>
                    <p class="blurb">
                        I'm Christine. I'm an undergrad at Columbia University in NYC studying computer science and linguistics. I am from San Francisco Bay Area and Shanghai. I love traveling, reading, dancing, and cooking.
                    </p>
                </div>
            </div> -->
            <!-- <img src="crbhamiltonbook.jpg" id="pichamiltonbook"/> -->
        </section>
        <section class="about">
            <div class="blurb">
                <h2>Learner. Researcher. Dancer.</h2>
                <p>I'm an undergrad at Columbia University in NYC studying computer science and linguistics. I am from San Francisco Bay Area and Shanghai. I love traveling, reading, dancing, and cooking.
                </p> 
            </div>
        </section>
        <!-- <section class="education">
            <h2>EDUCATION</h2>
        </section>
        <section class="experiences">
            <h2>EXPERIENCES</h2>
        </section>
        <section class="projects">
            <h2>PROJECTS</h2>
        </section> -->
        <section class="dance">
            <h1>DANCE</h1>
        </section>
        <section class="random">
            <h1>some random things</h1>
        </section>
        <section class="contact">
            <h1>CONTACT</h1>
        </section>

        <section class="footer">
            <a href="https://www.instagram.com/christinelitinghui" target="_blank" id="link">Instagram</a>
            <a href="https://www.github.com/tinghui2012" target="_blank" id="link">Github</a>
        </section>
    </div>
</template>

<style>
    *{
        box-sizing: border-box;
        margin: 0;
        padding: 0;
    }
    .main{
        margin: 0;
        padding: 0;
        background: #eee5e9;
        display: flex;
        flex-direction: column;
        font-family: 'Roboto Mono', monospace;
        font-size: 20px;
        justify-content: left;
        align-items: left;
        color: #432e36;
    }
    .navbar {
        z-index: 1;
        flex-direction: column;
        position: sticky;
        top: 0px;
        opacity: 100%;
        background-color: #eee5e9;
    }
    .navbaritems{
        padding: 0px;
        width: 100%;
        height: 100px;
        overflow: hidden;
        display: flex;
        justify-content: space-between;
        flex-direction: row;
        align-items: center;
    }
    a:link, a:visited, a:hover, a:active {
        text-decoration: none;
    }
    .navtabs a:hover, .navtabs a.active {
        background-color: #a6808c;
        
    }
    .navleft a {
        display: flex;
        padding: 0px;
        margin: 0px;
        vertical-align: middle;
        flex-direction: row;
        align-items: center;
    }
    #navbarlogo{
        padding: 0px;
        width: auto;
        height: 125px;
    }
    .navtabs{
        font-size: 20px;
        padding-right: 20px;
    }
    .navtabs a{
        float: left;
        padding: 15px;
        /* margin-left: 5px; */
        color: #432e36;
        font-size: 16px;
        width: auto;
        text-align: right;
        border: 2px solid #432e36;
        border-radius: 10px;
    }
    .navbarname{
        display: flex;
        float: left;
        padding: 10px;
        color: #432e36;
        font-size: 40px;
        width: auto;
        text-align: left;
        font-weight: bold;
        font-family: 'Roboto Mono', monospace;
        align-items: baseline;
    }
    .navtabs ul{
        margin: 0;
        align-items: right;
    }
    .navtabs li{
        font-family: 'Nunito', sans-serif;
        font-weight: 300;
        display: inline-flex;
        font-size: 15px;
    }
    .navdividerline{
        background-color: #432e36;
        height: 2px;
    }

    .mainimg{
        width: 100%;
        height: auto;
        top: 0;
        left: 0;
        opacity: 50%;
    }

    /* .section {
        position: fixed;
        color: #eee5e9;
        /* centers this div */
        /* left: 50%;
        top: 50%;
        transform: translate(-50%, -50%);
    } */ */
    .landing {
        padding: 0px;
    }
    .hello {
        background-image: url("/crbhamiltonsteps.jpg");
        height: 70vh;
    }
    .hello h1 {
        font-size: 40px;
        font-family: 'Roboto Mono', monospace;
        font-weight: 500;
    }
    /* .blurb div {
        background-color: #eee5e9;
        color: #432e36;
        text-align: center;
        padding: 50px;
        max-width: 300px;
    } */
    .blurb {
        align-content: center;
        justify-items: center;
    }
    .blurb h2 {
        font-size: 30px;
        margin-bottom: 10px;
        font-family: 'Dancing Script', cursive;
    }
    .section p {
        font-size: 20px;
        font-family: 'Nunito', sans-serif;
        line-height: 150%;
    }

    
    .mainbackgroundphoto{
        background-image: url(/crbhamiltonsteps.jpg);
        background-attachment: scroll;
    }
    section{
        padding: 50px;
    }
    /* .intro{
        flex-direction: column;
        padding-right: 50px;
    } */

    /* .homepageheading{
        font-size: 50px;
    }
    #pichamiltonbook{
        width: 30%;
        opacity: 0.5;
    }
    .homepagetext:hover{
        font-size: 18px;
    } */
</style>
