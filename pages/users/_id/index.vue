<template>
    <div class="card">
        <div class="card-image">
        <h1>Hello User Id : {{$route.params.id}}</h1>
        </div>
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
