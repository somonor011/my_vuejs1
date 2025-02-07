
<template>
    <div class="container">
        <label for="num1">Num1    </label>
        <input v-model="num1" type="text" name="" ref="num1">
        <label for="num2">Num2    </label>
        <input v-model="num2" type="text" name="" ref="num2">
        <div class="btn-blog">
            <button @click="Sum">+</button>
            <button @click="Min">-</button>
            <button @click="Mul">x</button>
            <button @click="Div">/</button>
            <button @click="ClearData" style="background-color: red; color: white;">AC</button>
        </div>
        <label for="total">Result </label>
        <input v-model="total" type="text" name="" ref="total">
    </div>
</template>

<script>
    // option API
    export default{

        data() {
            return {
                num1 : "",
                num2 : "",
                total : ""
            }
        },

        methods: {
            Sum(){
                this.total = Number(this.num1) + Number(this.num2);
            },

            Min(){
                this.total = Number(this.num1) - Number(this.num2);
            },

            Mul(){
                this.total = Number(this.num1) * Number(this.num2);
            },

            Div(){
                this.total = Number(this.num1) / Number(this.num2);
            },

            ClearData(){
                this.num1 = '';
                this.num2 = '';
                this.total = '';
            }
        },

    }
</script>
