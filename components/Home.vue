<script>
    export default{

    }
</script>
<template>
    <div class="main">
        <div class="navbar">
            <div class="navleft">CL</div>
            <ul class="navtabs">
                <li>ABOUT ME</li>
                <li>EDUCATION</li>
                <li>EXPERIENCES</li>
                <li>PROJECTS</li>
                <li>DANCE</li>
                <li>RANDOM</li>
                <li>CONTACT</li>
            </ul>
        
        </div>
        <section class="landing">
            <h1 class="greeting">Hello!</h1>
            <p class="blurb">
                I'm Christine. I'm an undergrad at Columbia studying computer science and linguistics. I am from San Francisco Bay Area and Shanghai. I love traveling, reading, dancing, and cooking.
            </p>
            <img src="crbhamiltonbook.jpg" id="pichamiltonbook"/>
        </section>

        <section class="aboutme">

        </section>
        <section class="education">
            
        </section>
        <section class="experiences">
            
        </section>
        <section class="projects">
            
        </section>
        <section class="dance">
            
        </section>
        <section class="lists">
            
        </section>
        <section class="contact">

        </section>

        <div class="footer">
            <a href="https://www.instagram.com/christinelitinghui" target="_blank" id="link">Instagram</a>
            <a href="https://www.github.com/tinghui2012" target="_blank" id="link">Github</a>
        </div>
    </div>
</template>

<style>
    *{
        box-sizing: border-box;
    }
    html{
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
        justify-content: center;
        align-items: center;
        color: #432e36;
    }
    .navtabs ul{
        margin: 0;
        align-items: right;
    }
    .navtabs li{
        display: inline-flex;
        font-size: 15px;
    }
    .homepageheading{
        font-size: 50px;
    }
    #pichamiltonbook{
        width: 80%;
        opacity: 0.5;
    }
    .homepagetext:hover{
        font-size: 18px;
    }
</style>
