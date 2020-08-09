<template>
    <b-navbar fixed-top="true" type="is-dark">
        <template slot="brand">
            <b-navbar-item tag="router-link" :to="{ path: '/' }">
                <img src="@/assets/images/pica.gif">
            </b-navbar-item>
        </template>
        <template slot="start">
            <b-navbar-item>
                <nuxt-link to="/profile" >Profile</nuxt-link>
            </b-navbar-item>
            <b-navbar-item>
                <nuxt-link to="/skill" >Skill</nuxt-link>
            </b-navbar-item>
            <b-navbar-item>
                <nuxt-link to="/products" >Products</nuxt-link>
            </b-navbar-item>
            <b-navbar-item>
                <nuxt-link to="/tmp" >Tmp</nuxt-link>
            </b-navbar-item>
            <div class="navbar-item">
  <div class="field is-grouped">
    <p class="control">
      <a class="button">
        <span class="icon">
          <font-awesome-icon icon="dollar-sign"  style="font-size: 30px"/>
        </span>
        <span>Tweet</span>
      </a>
    </p>
    <p class="control">
      <a class="button is-primary">
        <span class="icon">
          <i class="fas fa-download" aria-hidden="true"></i>
        </span>
        <span>Download</span>
      </a>
    </p>
  </div>
</div>
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