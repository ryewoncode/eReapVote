<template>
    <view class="view-menu">
        <view class="btn-menu"><text>참여</text></view>
        <view class="btn-menu"><text>등록</text></view>
        <view class="btn-menu"><text>승인</text></view>
        <view class="btn-menu"><text>제안</text></view>
        <view class="btn-menu"><text>결과</text></view>
    </view>
</template>


<script>
export default {
    
}
</script>

<style>
.view-menu {
    align-items: center;
    flex-direction: row;
    justify-content: space-between;
}

.btn-menu {
    border-width: 1;
    padding: 5px;
    margin: 10px;
}
</style>