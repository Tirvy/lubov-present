<template>
    <div class="slide-container">
        <div class="planet">
            <div class="bush1" />
            <div class="bush2" />
            <div class="bush3" />
            <div class="bush4" />
        </div>

        <div class="lubov-captain"></div>
        <div class="bush3 given" />
        <div class="zays"></div>
        <div class="bush2 given1" />
        <div class="bush2 given2" />
        <div class="bush2 given3" />
    </div>
</template>

<script>
export default {
    
}
</script>

<style scoped lang="scss">
.slide-container {
    background: url('~@/assets/space.jpg') no-repeat center;
    background-size: cover;
}

.planet {
    background: url('~@/assets/planet.png') no-repeat center;
    background-size: contain;
    width: 1400px;
    height: 1400px;

    position: absolute;
    left: 5%;
    top: -20%;
    transform: rotate(45deg);
}

.lubov-captain {
    background: url('~@/assets/captain.png') no-repeat center;
    background-size: contain;
    width: 100px;
    height: 210px;
    position: absolute;
    bottom: 200px;
    left: 380px;
}

.zays {
    background: url('~@/assets/zays.png') no-repeat center;
    background-size: contain;
    width: 170px;
    height: 240px;
    position: absolute;
    bottom: 200px;
    left: 510px;
}

.bush1 {
    background: url('~@/assets/bush1.png') no-repeat center;
    top: 50%;
    left: 5%;
    transform: rotate(-65deg);
}

.bush2 {
    background: url('~@/assets/bush2.png') no-repeat center;
    top: 50%;
    left: 58%;
    transform: rotate( 75deg);
    &.given1 {
        transform: rotate(-5deg);
        top: 63%;
        left: 29%;
    }
    &.given2 {
        transform: rotate(-5deg);
        top: 63%;
        left: 35%;
    }
    &.given3 {
        transform: rotate(-5deg);
        top: 63%;
        left: 42%;
    }
}

.bush3 {
    background: url('~@/assets/bush3.png') no-repeat center;
    top: 83%;
    left: 38%;
    transform: rotate( 165deg);
    &.given {
    transform: rotate(45deg) scaleX(-1);
    top: 46%;
    left: 33%;
        filter: drop-shadow(2px 2px 0 white) 
                drop-shadow(-2px -2px 0 white);
    }
}

.bush4 {
    background: url('~@/assets/bush4.png') no-repeat center;
    top: 78%;
    left: 14%;
    transform: rotate(226deg) scale(2.5);
}

.bush1,
.bush2,
.bush3,
.bush4 {
    width: 15%;
    height: 15%;
    background-size: contain;
    position: absolute;
}
</style>