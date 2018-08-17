<template>
<div>

        <div class="panel-block">
            <div class="column is-four-fifths">
                <p class="control has-icons-left"> 
                <input class="input is-small" type="text" v-model="userId" placeholder="search">
                <span class="icon is-small is-left">
                </span>
                </p>
            </div>

        <button class="button is-link is-outlined" @click="onLoadUser">Load User</button>
            </div>
        <br>
        <nuxt-child/>
  </div>

</template>
<script>
export default {
    data(){
        return{
            userId: ''
        }
    },
    methods: {
        onLoadUser(){
            this.$router.push('/users/'+this.userId )
        }
    },
    layout: 'users'

}
</script>
<style>

</style>
