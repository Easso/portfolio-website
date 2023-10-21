<template>
    <div class="wrapper">
        <div class="main-container">
            <div class="container-one">
                <div class="profile">
                    <img src="../assets/PFP.jpg" alt="">
                    <h3>Easson Weisshaar</h3>
                    <p>Electrical Engineering Student</p>
                </div>
                <div class="social-links">
                    <div class="accounts">
                    <a href="https://github.com/Easso" target="_blank">
                        <img href="https://github.com/Easso" src="../assets/github-mark.svg" alt="" target="_blank"> 
                        <h2>GitHub</h2>
                    </a>
                    </div>
                    <div class="accounts">
                    <a href="https://www.linkedin.com/in/easson" target="_blank">
                        <img href="https://www.linkedin.com/in/easson" src="../assets/iconmonstr-linkedin-3.svg" alt="" target="_blank">
                        <h2>LinkedIn</h2>
                    </a>
                    </div>  
                </div>
            </div>
            <div class="container-two">
                <div class="about-me">
                    <h1 class="right-title">About Me</h1>
                    <p>
                        I am currently a third year electrical engineering coop student studying at the University of Waterloo.
                        My professional interests lie in AI/ML, embedded, and front-end development. My current goal is to find a 
                        way to combine my passion for hockey with one of the previously mentioned fields. Whether it is establishing 
                        a sport-related data science club at school, creating a predicative data modeling tool to help me win in 
                        fantasy hockey, or developing physical hcokey training tools.
                    </p>
                </div>
                <div class="skills">
                    <h1 class="right-title">Skills</h1>
                    <div class="logos">
                        <img src="../assets/cpp_logo.svg" alt="">
                        <img src="../assets/vue_logo.svg" alt="">
                        <img src="../assets/python-seeklogo.com.svg" alt="">
                    </div>
                </div>
                <div class="button-container">
                    <div class="projects-button">
                        <a href="">My Projects</a>
                    </div>
                    <div class="projects-button">
                        <a href="">My Resume</a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>

</script>

<style scoped>
.wrapper{
    display: flex;
    justify-content: center;
}
    img {
        height: 20px
    }
    .main-container {
        margin-top: 5%;
        display: flex;
        flex-direction: row;
        background-color:#3c5148;
        border-radius: 25px;
        box-shadow: rgba(0,0,0,0.75) 0px 3px 18px;
        width: 60%;
        margin-bottom: 1.5rem;
    }
    .container-one{
        background-color: #b2c5b2;
        padding:2.5%;
        width:40%;
        border-top-left-radius: 15px;
        border-bottom-left-radius: 15px;
        box-shadow: rgba(0,0,0,0.24) 0px 3px 8px;
        color: #3c5148;
    }
    .profile img{
        height: 8rem;
        border-radius: 40%;
    }
    .accounts {
        padding-inline: 1.4rem;
    }
    .accounts a {
        text-decoration: none;
        color: #2c3e50;
        font-size: 10px;
    }
    .social-links {
        display: flex;
        flex-direction: row;
        justify-content:center;
    }
    .social-links img {
        height: 3rem;
    }
    .right-title{
        display: flex;
        justify-content: center;
        margin-bottom: 3%;
        font-family:serif;
        color: #b2c5b2;
    }
    .container-two{
        padding:2.5%;
        border-radius: 25px;
        background-color: #3c5148;
        margin: 2.5%;
        width: 60%
        
    }
    .about-me{
        text-align: left;
        color: #b2c5b2;
    }
    .title{
        display: flex;
        justify-content: center;
        margin-bottom: 3%;
        font-family:serif;
        color: #1b2727;
    }
    .logos {
        display:flex;
        justify-content: center;       
    }
    .logos img {
        height: 2.5rem;
    }
    .button-container{
        margin-top: 5%;
        display:flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;
    }
    .projects-button{
        background-color:#6b8e4e;
        margin: 5px;
        padding: 5px;
        border-radius: 15px;
    }
    .projects-button a{
        text-decoration: none;
        color: #2c3e50;
        color: #d5dddf;
    }
    @media only screen and (max-width: 950px) {
        .main-container{
            width: 98%;
        }
        .accounts{
            display: flex;
            padding-inline: 0.5rem;
        }
    }
</style>