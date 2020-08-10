<template>
    <b-navbar fixed-top="true" type="is-dark">
        <template slot="brand">
            <b-navbar-item tag="router-link" :to="{ path: '/' }">
                <img src="@/assets/images/pica.gif">
            </b-navbar-item>
        </template>
        <template slot="start">
            <b-navbar-item>
                <nuxt-link to="/profile" >
                    <font-awesome-icon icon="address-card"/> Profile 
                </nuxt-link>
            </b-navbar-item>
            <b-navbar-item>
                <nuxt-link to="/skill" >
                    <font-awesome-icon icon="laptop-code"/> Skill 
                </nuxt-link>
            </b-navbar-item>
            <b-navbar-item>
                <nuxt-link to="/products" >
                    <font-awesome-icon icon="server"/>Products 
                </nuxt-link>
            </b-navbar-item>
            <b-navbar-item>
                <nuxt-link to="/tmp" ><img src="@/assets/images/pica.gif">Tmp</nuxt-link>
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