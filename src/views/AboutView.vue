<template>
    <div class="about-container flex w-full justify-content-center align-content-center">
        <div class="about-content mx-auto my-8 flex flex-column">
            <div class="flex flex-row gap-4">
                <div>
                    <img src="../assets/images/pp.jpg" alt="" height="450">
                </div>
                <div>
                    <header class="about-header">
                        <span>Hey there! </span>
                        <br>
                        <span>I'm <span class="name">Bryan Arnoco</span>,
                            <br> a Computer Engineering student
                            <br> and Aspiring Web Developer.</span>
                    </header>
                    <p class="about-p">
                        In my spare time, I've been engaging in website development as a hobby, experimenting with various
                        frameworks for both front-end and back-end development. Being passionate about creating things, I
                        constantly seek to challenge myself, pushing the boundaries to enhance my skills and achieve more.
                    </p>
                </div>
            </div>
            <div>
                <p class="about-quote">"Live each day as if it were your final opportunity to make a lasting impact."</p>
            </div>
            <div class="flex flex-row justify-content-center">
                <div class="about-box-skills flex flex-column justify-content-center p-3 text-center gap-3">
                    <CodeIcon class="icon" height="80px" />
                    <span>1 project developed</span>
                    <span>Vue.js developer</span>
                </div>
                <div class="about-box-skills flex flex-column justify-content-center p-3 text-center gap-3">
                    <BookIcon class="icon" height="80px" />
                    <span>Web Development Intern at </span>
                    <span>Lanex Corporation</span>
                </div>
            </div>
            <div class="flex flex-column justify-content-center">
                <header>
                    <h1 class="hobbies-header">Hobbies and Interests</h1>
                </header>
                <div class="flex flex-row gap-8 justify-content-center">
                    <div class="hobbies-ea flex flex-column justify-content-center text-center">
                        <BasketballIcon class="ball" height="100px" />
                        <span class="hobbies-label ">Basketball</span>
                    </div>
                    <div class="hobbies-ea flex flex-column justify-content-center text-center">
                        <VolleyballIcon class="ball" height="100px" />
                        <span class="hobbies-label ">Volleyball</span>
                    </div>
                    <div class="hobbies-ea flex flex-column justify-content-center text-center">
                        <GamingIcon class="ball" height="100px" />
                        <span class="hobbies-label ">Gaming</span>
                    </div>
                    <div class="hobbies-ea flex flex-column justify-content-center text-center">
                        <SingingIcon class="ball" height="100px" />
                        <span class="hobbies-label ">Singing</span>
                    </div>
                    <div class="hobbies-ea flex flex-column justify-content-center text-center">
                        <MusicIcon class="ball" height="100px" />
                        <span class="hobbies-label ">Listening to Music</span>
                    </div>
                </div>

            </div>
            <div class="contact-container flex flex-row ">
                <div class="logo-container flex flex-column justify-content-center text-center">
                    <img src="../assets/images/Logo.png" alt=""
                        height="150">
                    <span class="logo-label">bwy</span>
                </div>
                <div class="text-center w-full">
                    <header class="contact-header">Contact Info</header>
                    <div class="contact-details flex flex-column mt-4">
                        <span>Bryan M. Arnoco</span>
                        <span>Yati, Liloan, Cebu, Philippines</span>
                        <span>arnoco42@gmail.com</span>
                        <span>+639216768250</span>
                    </div>
                </div>
                
            </div>
        </div>
    </div>
</template>
<script setup>
import CodeIcon from '../components/icons/CodeIcon.vue';
import BookIcon from '../components/icons/BookIcon.vue';
import BasketballIcon from '../components/icons/BasketballIcon.vue';
import VolleyballIcon from '../components/icons/VolleyballIcon.vue';
import GamingIcon from '../components/icons/GamingIcon.vue';
import SingingIcon from '../components/icons/SingingIcon.vue'
import MusicIcon from '../components/icons/MusicIcon.vue'

</script>
<style>
.about-container {
    width: fit-content;
    background: linear-gradient(#896fbb, #6d5932);
    background-position: center;
    background-size: cover;
    background-blend-mode: darken;
    background-attachment: fixed;
    overflow: auto;
}

.about-content {
    width: 1000px;
}

.about-header {
    color: rgb(75, 51, 51);
    font-size: 40px;
    font-family: 'Fira Code', monospace;
}

.about-p {
    font-size: 14px;
    width: 600px;
    text-align: justify;
    text-justify: inter-word;
    line-height: 2;
    font-family: 'Roboto', sans-serif;
}

.about-quote {
    font-family: "Lucida Console", "Courier New", monospace;
    font-size: 70px;
    font-style: italic;
    text-align: center;
    line-height: 1;
    color: rgb(43, 36, 104);
}

.about-box-skills {
    height: 250px;
    width: 250px;
    background: linear-gradient(rgba(148, 36, 36, 0.5), rgba(89, 77, 155, 0.5));
    box-shadow: 0 0 18px 2px #b28fce;
    margin: 20px;
    border-radius: 25px;
    color: white;
    font-family: 'Fira Code', monospace;
    transition: 0.5s;
}

.about-box-skills:hover {
    color: rgb(11, 189, 11);
    background: linear-gradient(rgba(141, 89, 89, 0.5), rgba(73, 62, 136, 0.5));
}

.about-box-skills:hover .icon {
    fill: white;
}

.icon {
    fill: rgb(11, 189, 11);
}

.hobbies-header {
    color: transparent;
    background: linear-gradient(to right, #461212, #00f000);
    background-clip: text;
    -webkit-background-clip: text;
    font-size: 100px;
}

.hobbies-ea {
    height: 150px;
}

.hobbies-label {
    font-size: 30px;
    color: white;
    font-family: 'Fira Code', monospace;
}

.ball {
    fill: white;
    transition: 0.5s;
}

.ball:hover {
    fill: rgb(11, 189, 11);
    animation: spin 2s linear infinite;
}

@keyframes spin {
    0% {
        transform: rotate(0deg);
    }

    100% {
        transform: rotate(360deg);
    }
}

.contact-container {
    margin-top: 40px;
    height: 200px;
    background: linear-gradient(rgba(148, 36, 36, 0.5), rgba(89, 77, 155, 0.5));
    box-shadow: 0 0 18px 2px #b28fce;
    border-radius: 10px;
}

.contact-container:hover {
    background: linear-gradient(rgba(141, 89, 89, 0.5), rgba(73, 62, 136, 0.5));
}
.logo-label {
    color: #00f000;
    font-size: 25px;
    font-family: 'Fira Code', monospace;
}
.logo-container {
    border-right: 1px solid;
    margin: 10px;
}

.contact-header {
    font-size: 40px;
}

.contact-details {
    font-size: 20px;
    color: white;
}
</style>