<template>
    <div class="notification is-primary">
  <button class="delete"></button>
  <h2><strong>Hello My User Id is - {{$route.params.id}}</strong></h2>
</div>
</template>
<script>
export default {
    validate(data){
        //ragex test
        console.log(/^\d+$/.test(data.params.id))
        return /^\d+$/.test(data.params.id)

        // if(typeof(data.params.id) === "string"){
        //     console.log('miew')
        // }
        // console.log(typeof(data.params.id))
        // return true
    }
}
</script>
<style>

</style>
