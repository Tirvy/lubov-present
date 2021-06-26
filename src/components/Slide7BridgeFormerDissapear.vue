<template>
    <div class="slide-container">
        <div class="planet"></div>
        <div class="former"></div>
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
    opacity: 0.8;

    animation: spin 50s infinite linear;
}

.former {
    background: url('~@/assets/former.png') no-repeat center;
    background-size: contain;
    width: 200px;
    height: 200px;
    position: absolute;
    left: 40%;
    top: 30%;
    animation: shake 2s infinite;
}

$distance: 1;

.bridge {
    background: url('~@/assets/bridge.png') no-repeat center;
    background-size: contain;
    width: 100%;
    height: 100%;
    position: absolute;
}

.lubov-captain {
    background: url('~@/assets/captain.png') no-repeat center;
    background-size: contain;
    width: 100px * $distance;
    height: 210px * $distance;
    position: absolute;
    bottom: 0;
    left: 200px;
}
</style>