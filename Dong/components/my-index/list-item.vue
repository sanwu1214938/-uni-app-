<template>
	
    <view class="list-item index">
        dong-list-item
		<navigator url="../../pages/test/test/test">test页面</navigator>
    </view>
	
</template>

<script>
    export default {
		data() {
			return {
				msg: "dong"
			}
		},
        methods: {
            
        }
    }
</script>

<style scoped>
	.list-item{
		width: 100%;
		height: 120rpx;
		display: flex;
		flex-direction: row;
		justify-content: center;
		align-items: center;
		border: #007AFF 1px solid;
	}
</style>
