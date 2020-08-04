<template>
    <b-navbar>
        <template slot="brand">
            <b-navbar-item tag="router-link" :to="{ path: '/' }">
                <!-- <img
                    src="https://raw.githubusercontent.com/buefy/buefy/dev/static/img/buefy-logo.png"
                    alt="Lightweight UI components for Vue.js based on Bulma"
                > -->
                <img src="@/assets/images/pica.gif">
            </b-navbar-item>
        </template>
        <template slot="start">
            <b-navbar-item>
                <nuxt-link to="/profile" >profile</nuxt-link>
            </b-navbar-item>
            <b-navbar-item>
                <nuxt-link to="/skill" >skill</nuxt-link>
            </b-navbar-item>
            <b-navbar-item>
                <nuxt-link to="/products" >products</nuxt-link>
            </b-navbar-item>
        </template>

        <!-- <template slot="end">
            <b-navbar-item>
                <nuxt-link to="/profile" >profile</nuxt-link>
            </b-navbar-item>
            <b-navbar-item>
                <nuxt-link to="/tmp" >skill</nuxt-link>
            </b-navbar-item>
            <b-navbar-item>
                <nuxt-link to="/tmp" >output</nuxt-link>
            </b-navbar-item>
        </template> -->
    </b-navbar>
</template>