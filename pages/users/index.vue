<template> 
    <div class="container">
        <nuxt-link to="/">BACK</nuxt-link>
        <div class="m-5"></div>
        <div class="form-group">
          <input type="text"
            class="form-control" aria-describedby="helpId" placeholder=""
            v-model="userId">
           <button @click="onLoadUser" class="btn btn-outline-dark btn-block">
                Load User
           </button>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            userId: ''
        }
    },
    methods: {
        onLoadUser() {
            this.$router.push('/users/' + this.userId)
        }
    }
}
</script>
