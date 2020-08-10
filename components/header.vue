<template>
    <b-navbar fixed-top="true" type="is-info">
        <template slot="brand">
            <b-navbar-item tag="router-link" :to="{ path: '/' }">
                <img src="@/assets/images/pica.gif">
            </b-navbar-item>
        </template>
        <template slot="start">
            <b-navbar-item href="/profile">
                <font-awesome-icon icon="address-card"/> Profile 
            </b-navbar-item>
            <b-navbar-item href="/skill">
                <font-awesome-icon icon="laptop-code"/> Skill 
            </b-navbar-item>
            <b-navbar-item href="/products">
                <font-awesome-icon icon="server"/>Products 
            </b-navbar-item>
            <b-navbar-item href="/tmp">
                <img src="@/assets/images/pica.gif">Tmp
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