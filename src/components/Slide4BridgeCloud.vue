<template>
    <div class="slide-container">
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
    background: url('~@/assets/cloud.jpg') no-repeat center;
    background-size: cover;
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