<template>
    <h1>MENU</h1>

    <p v-for="m in menu" :key="m.day" @click="m.show = !m.show">
        <b>{{ m.day }}</b> <br />
        <i v-if="m.show">{{ m.food }}</i>
    </p>

    <img class="menu-logo" alt="menu Logo" src="../assets/Menu.jpg">
    
</template>

<script>
export default {
    data(){
        return {
            menu:[
                {
                    day: "Monday",
                    food: "Chicken Alfredo Pasta with fresh broccoli and parmesan.",
                    show: false
                },
                {
                    day: "Tuesday",
                    food: "Vegetarian Quinoa Salad with roasted vegetables and halloumi.",
                    show: false
                },
                {
                    day: "Wednesday",
                    food: "Swedish Meatballs with cream sauce, mashed potatoes, and lingonberry jam.",
                    show: false
                },
                {
                    day: "Thursday",
                    food: "Thai Red Curry with chicken, vegetables, and jasmine rice.",
                    show: false
                },
                {
                    day: "Friday",
                    food: "Grilled Salmon with lemon and herb sauce, served with roasted vegetables and wedge potatoes.",
                    show: false
                },
            ]
        }
    }
}
</script>

<style scoped>
.menu-logo {
    max-width: 30%;
    margin-bottom: 20px;
}
</style>