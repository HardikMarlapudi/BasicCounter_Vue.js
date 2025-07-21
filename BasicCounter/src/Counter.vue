<template>
    <h1 id="title">Counter Program</h1>
    <p id="counter">Counter: {{count}}</p>
    <div class="buttons">
        <button id="increment" v-on:click="increment()">Increment</button>
        <button id="reset" v-on:click="reset()">Reset</button>
        <button id="decrement" v-on:click="decrement()">Decrement</button>
    </div>
</template>


<script>
export default {
    data() {
        return {
            count: 0
        }
    },

    methods: {
        increment() {
            this.count++;
        },

        reset() {
            this.count = 0
        },

        decrement() {
            this.count --;
        }
    }
}
</script>

<style>
    #title {
        text-align: center;
        font-size: 30px;
        font-family: 'Courier New', Courier, monospace;
    }

    #counter {
        text-align: center;
        font-size: 20px;
        font-family: 'Courier New', Courier, monospace;
    }

    .buttons {
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 5px;
    }

    #increment {
        background-color: lightgreen;
        font-size: 20px;
        font-family: 'Courier New', Courier, monospace;
        font-weight: bold;
        border-radius: 5px;
        border-color: lightgreen;
        cursor: pointer;
    }

    #reset {
        background-color: lightblue;
        font-size: 20px;
        font-family: 'Courier New', Courier, monospace;
        font-weight: bold;
        border-radius: 5px;
        border-color: lightblue;
        cursor: pointer;
    }

    #decrement {
        background-color: red;
        font-size: 20px;
        font-family: 'Courier New', Courier, monospace;
        font-weight: bold;
        border-radius: 5px;
        border-color: red;
        cursor: pointer;
    }
    
</style>
