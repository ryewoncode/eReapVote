<template>
    <view class="header">
        <view class="header-left">
            <touchableOpacity :on-press="showAlert">
                <image id="logo" :source="require('../../assets/image/logo.png')"  />
            </touchableOpacity>
            <text class="title"> {{ title }}</text>
        </view>
        <view class="header-right">
            <text-input class="search-input" />
            <touchableOpacity :on-press="showAlert">
                <image id="search" :source="require('../../assets/image/search.png')"  />
            </touchableOpacity>
            <touchableOpacity :on-press="showAlert">
                <image id="menu" :source="require('../../assets/image/menu.png')"  />
            </touchableOpacity>
        </view>
    </view>
</template>

<script>
import { Alert } from "react-native"

export default {
    props: ['title'],
    methods: {
        showAlert: function() {
            Alert.alert(
                'Alert Title',
                'My Alert Msg',
                [
                    {text: 'Ask me later', onPress: () => console.log('Ask me later pressed')},
                    {text: 'Cancel', onPress: () => console.log('Cancel Pressed'), style: 'cancel'},
                    {text: 'OK', onPress: () => console.log('OK Pressed')},
                ],
                { cancelable: false }
            );
        }
    }
}
</script>

<style>
.header {
    height: 50px;
    background-color: #FFFFFF;
    /* justify-content: flex-start;
    align-items: flex-start; */
    align-items: center;
    flex-direction: row;
    padding: 5px;
}
.header-left {
    flex: 1;
    flex-direction: row;
    align-items: flex-start;
}
.header-right {
    flex: 2;
    flex-direction: row;
    align-items: flex-end;
    text-align: right;
}
.header-right image {
    margin-left: 5px;
    margin-right: 5px;
}

.title {
    color: black;
    font-size: 20px;
    font-weight: 500;
}
.search-input {
    flex: 1;
    height: 30px;
    width: auto;
    min-width: 100px;
    border-width: 1;
    margin-right: 5px;
}
</style>