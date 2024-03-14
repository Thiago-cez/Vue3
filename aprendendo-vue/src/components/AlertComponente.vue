<template>
    <div :class="base"> Seu Formulario foi enviado Com Sucesso 
        
    </div>
</template>

<script>
   export default {
    data() {},
    props: [ 'variant'],
    computed: {
        base() {
            return [ 
                'alert',
                this.variant ? `alert-${this.variant} ` : ""
            ]
        }
    }
   }

</script>


<style scoped>
.alert {
    padding: 5px;
    border-radius: 6px;
    color: gray;
    background:#ddd
}

.alert-sucess {
    background-color: green;
    color: white;
}
.alert-danger {
    background-color: yellow;
    color: black;
}
.alert-denied {
   background-color: red;
   color: white   
}
</style>