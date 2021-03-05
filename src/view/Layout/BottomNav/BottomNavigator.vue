<template>
    <view class="view-bottomNav">
        <!-- <button title="홈" />
        <button title="알림" />
        <button title="설정" />
        <button title="마이페이지" /> -->
        <view>
            <touchableOpacity>
                <image id="home" :source="require('../../../assets/image/home.png')"  />
            </touchableOpacity>
        </view>
        <view>
            <touchableOpacity>
                <image id="notice" :source="require('../../../assets/image/notice.png')"  />
            </touchableOpacity>
        </view>
        <view>
                <touchableOpacity>
                    <image id="setting" :source="require('../../../assets/image/setting.png')"  />
                </touchableOpacity>
        </view>
        <view>
            <touchableOpacity>
                <image id="mypage" :source="require('../../../assets/image/mypage.png')"  />
            </touchableOpacity>
        </view>
    </view>
</template>

<script>

export default {
    
}
</script>

<style>
.view-bottomNav {
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    height: 60px;

}

.view-bottomNav view {
    flex: 1;
    justify-content: space-between;
    text-align: center;
}
</style>