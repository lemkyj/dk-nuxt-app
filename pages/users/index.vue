<template> 
    <div class="container">
        <div class="form-group">
          <input type="text"
            class="form-control" aria-describedby="helpId" placeholder=""
            v-model="userId">
           <button class="btn btn-outline-dark btn-block">
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
        onLoadUser() 
    }
}
</script>
