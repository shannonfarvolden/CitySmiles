<template>
    <b-navbar variant="light">
        <b-navbar-brand :to="{ name: 'home'}">
            <img :src="logo" v-b-tooltip.hover title="Smile :)" v-b-tooltip.html.top>
        </b-navbar-brand>
        <b-navbar-nav class="ml-auto">
            <b-nav-item :to="{ name: 'createOrganization' }" v-b-tooltip.hover title=":D" v-b-tooltip.html.top>Add Your Organization</b-nav-item>
            <b-nav-item :to="{ name: 'organizations' }" v-b-tooltip.hover title=";)">All Organizations</b-nav-item>
        </b-navbar-nav>
    </b-navbar>
</template>
    
<script>
export default {
  name: 'Navbar',
   data(){
    return {
      logo: require('./assets/logo.png'),
    }
  }
}
</script>