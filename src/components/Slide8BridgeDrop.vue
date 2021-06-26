<template>
    <div class="slide-container">
        <div class="planet">
            <div class="bush1" />
            <div class="bush2" />
            <div class="bush3" />
            <div class="bush4" />
        </div>
        <div class="bridge">
            <div class="lubov-captain"></div>
        </div>
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
    width: 600px;
    height: 600px;

    position: absolute;
    left: 30%;
    top: 0;

    animation: spin 50s infinite linear;
}

$distance: 1;

.bridge {
    background: url('~@/assets/bridge.png') no-repeat center;
    background-size: contain;
    width: 100%;
    height: 100%;
    position: absolute;
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
}

.bush3 {
    background: url('~@/assets/bush3.png') no-repeat center;
    top: 83%;
    left: 38%;
    transform: rotate( 165deg);
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