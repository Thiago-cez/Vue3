<template>
    <div :class="base"> 
        <slot />

        <button @click="fecharAlerta()"> X </button>
    </div>
</template>

<script>
   export default {
    data() {},
    props: {
        variant: {
            type: String,
            default: ""
        }
    },
    computed: {
        base() {
            return [ 
                'alert',
                this.variant ? `alert-${this.variant} ` : ""
            ]
        }
    },
    methods: {
        fecharAlerta() {
            this.$emit('fechar')
        }
    }
   }

</script>


<style scoped>
.alert {
    display: flex;
    justify-content: space-between;
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
import { emit } from 'nodemon';
