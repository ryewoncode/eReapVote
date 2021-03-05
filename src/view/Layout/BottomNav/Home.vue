z<template>
    <scroll-view class="view-container" :content-container-style="{contentContainer: {paddingVertical: 20}}">
        <view>
            <title title="퀵메뉴 >" />
            <quick-menu />
        </view>        
        <view>
            <title title="<진행중인 투표>" :style="{alignItems: 'center'}" />
            <progress-voting />
        </view>   
        <view>
            <title title="투표 리스트 >" />
            <view><text>투표 리스트</text></view>
        </view>
        <view>
            <title title="의견 제안 >" />
            <view><text>의견 제안</text></view>
        </view>
        <view>
            <title title="투표 결과 >" />
            <view><text>투표 결과</text></view>
        </view>
    </scroll-view>
</template>

<script>
import Title from "../../../components/Title"
import QuickMenu from "../../../components/Home/QuickMenu"
import ProgressVoting from "../../../components/Home/ProgressVoting"

export default {
    components: {
        Title,
        QuickMenu,
        ProgressVoting
    }    
}
</script>

        ProgressVoting
<style>

</style>