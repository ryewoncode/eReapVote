<template>
    <view>
        <text class="text-title">{{ title }}</text>
    </view>
</template>

<script>
export default {
    props: [ 'title' ]
}
</script>

<style>
.text-title {
    color: black;
    font-weight: 500;
    font-size: 15px;
}
</style>