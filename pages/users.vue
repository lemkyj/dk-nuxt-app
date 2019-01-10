<template>
    <div class="container">
        <div class="form-group">
          <input type="text"
            class="form-control" aria-describedby="helpId" placeholder=""
            v-model="userId">
           <button @click="onLoadUser" class="btn btn-outline-dark btn-block">
                Load User
           </button>
        </div>
        <nuxt-child />
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
