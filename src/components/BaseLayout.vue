<template>
    <div class="container">
        <RouterView />
        <div class="flex justify-content-center">
            <div class="navbar">
                <div class="flex flex-row gap-4 m-auto">
                    <div class="nav-buttons">
                        <div class="flex m-auto">
                            <router-link to="/">Home</router-link>
                        </div>
                    </div>
                    <div class="nav-buttons">
                        <div class="flex m-auto">
                            <router-link to="/about">About Me</router-link>
                        </div>
                    </div>
                    <div class="nav-buttons">
                        <div class="flex m-auto">
                            <router-link to="/projects">Projects</router-link>
                        </div>
                    </div>
                </div>
            </div>
        </div>

    </div>
</template>