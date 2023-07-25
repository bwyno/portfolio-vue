<template>
    <div class="flex h-full w-full justify-content-center align-content-center ">
        <div class="m-auto flex flex-row gap-4">
            <div>
                <img src="../assets/images/me.jpg" alt="" height="600">

            </div>
            <div class="welcome-msg ">
                <span class="header-text">#hi-i-am-<span class="name">Bryan</span>&<span class="name">Arnoco</span>!</span>
                <br>
                <span class="work-title">Aspiring Web <br> Developer</span>
                <br>
                <p class="home-p">
                    Welcome to my Web Development Journey! I am <span class="name">Bryan Arnoco</span>, an aspiring web
                    developer, and this website serves as a documentation of my work, progress, and passion for creating
                    dynamic digital experiences. Join me in exploring the world of web technologies, from the fundamentals
                    of HTML and CSS to the intricacies of JavaScript and beyond. Let's inspire, learn, and grow together as
                    we shape the future of the web, one line of code at a time. Happy coding!
                </p>
            </div>
        </div>
    </div>
</template>
<script setup>

</script>

<style>
.welcome-msg {
    font-family: 'Roboto', sans-serif;
}

.header-text {
    color: rgb(172, 170, 170);
    font-size: 40px;
}

.name {
    color: rgb(6, 255, 6);
}

.work-title {
    font-size: 100px;
    font-weight: bold;
}

.home-p {
    font-size: 14px;
    width: 600px;
    text-align: justify;
    text-justify: inter-word;
    line-height: 2;
    transition: 0.5s;
    color: rgb(99, 59, 59);
}

.home-p:hover {
    font-size: 19px;
    color: #271f38;
    font-weight: 600;
}
</style>