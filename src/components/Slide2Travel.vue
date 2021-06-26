<template>
    <div class="slide-container">
        <div class="ship">
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

.ship {
    background: url('~@/assets/ship.png') no-repeat center;
    background-size: contain;
    width: 400px;
    height: 400px;
    position: absolute;
    top: 200px;
    left: 200px;
    animation: sway 5s infinite;
}

.lubov-captain {
    background: url('~@/assets/captain.png') no-repeat center;
    background-size: contain;
    width: 70px;
    height: 50px;
    position: absolute;
    top: 172px;
    left: 133px;
}
</style>