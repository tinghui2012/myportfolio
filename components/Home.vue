<script>
    export default{

    }
</script>
<template>
    <div class="main">
        <div class="navbar">
            <div class="navleft">
                <a href=".about" class="jumptotop"><img src="CLlogotrans.png" id="navbarlogo" alt="logo"/>
                <div class="navbarname">CHRISTINE LI</div></a>
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
        <section class="about">
            <div class="intro">
                <div class="introleft">
                    <h1 class="greeting">Hello!</h1>
                    <p class="blurb">
                        I'm Christine. I'm an undergrad at Columbia studying computer science and linguistics. I am from San Francisco Bay Area and Shanghai. I love traveling, reading, dancing, and cooking.
                    </p>
                    <br/>
                </div>
            </div>
            <img src="crbhamiltonbook.jpg" id="pichamiltonbook"/>
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
            <h2>DANCE</h2>
        </section>
        <section class="random">
            <h2>some random things</h2>
        </section>
        <section class="contact">
            <h2>CONTACT</h2>
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
        font-family: Georgia, 'Times New Roman', Times, serif;
        font-size: 20px;
        justify-content: left;
        align-items: left;
        color: #432e36;
    }
    .navbar{
        padding: 20px;
        width: 100%;
        height: 100px;
        overflow: auto;
        display: flex;
        justify-content: space-between;
    }
    .navbar a:hover{
        background-color: #a6808c;
        
    }
    .navbar a.active {
        background-color: #a6808c;
    }

    .navleft a{
        display: flex;
        flex-direction: row;
    }
    .navbarname{
        display: flex;
        justify-content: space-between;
    }
    .navtabs{
        font-size: 8px;
    }
    .navtabs a{
        float: left;
        padding: 12px;
        color: #432e36;
        font-size: 16px;
        width: auto;
        text-align: right;
    }
    .navbarname{
        float: left;
        padding: 16px;
        color: #432e36;
        font-size: 20px;
        width: auto;
        text-align: right;
        font-weight: bold;
        text-decoration: wavy;
    }
    #navbarlogo{
        width: 50px;
    }
    .navtabs ul{
        margin: 0;
        align-items: right;
    }
    .navtabs li{
        display: inline-flex;
        font-size: 15px;
    }
    section{
        padding: 50px;
    }
    .about{
        display: flex;
    }
    .intro{
        flex-direction: column;
        padding-right: 50px;
    }

    .homepageheading{
        font-size: 50px;
    }
    #pichamiltonbook{
        width: 30%;
        opacity: 0.5;
    }
    .homepagetext:hover{
        font-size: 18px;
    }
</style>
