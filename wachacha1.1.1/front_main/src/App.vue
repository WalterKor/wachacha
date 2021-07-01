<template>
    <div class="background">
        <div class="backScreen">
            <img :src="screen[0].first" />
        </div>
        <div class="redBox"></div>
        <!-- <img :src="screen[0].second" /> -->
        <!-- <img src="./assets/main/first.jpg" /> -->
    </div>
</template>

<script>
export default {
    name: "App",
    components: {},
    data() {
        return {
            screen: [
                {
                    first: require("@/assets/main/first.jpg"),
                    second: require("@/assets/main/second.jpg"),
                    third: require("@/assets/main/third.png"),
                },
            ],
        };
    },
};
</script>

<style>
.background {
    position: absolute;
    width: 100%;
    height: 100%;
    margin: 0px;
    padding: 0px;
    box-sizing: border-box;
}
.backScreen {
    position: relative;
    width: 100px;
    height: 100px;
    margin: 0px;
    padding: 0px;
}
.redBox {
    width: 100px;
    height: 100px;
    margin: 0px;
    padding: 0px;
    background-color: red;
}
</style>
