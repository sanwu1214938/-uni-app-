<template>

	<view class="list-page">

		<uni-list class="listview" :enableBackToTop="true" :scroll-y="true">

			<listItem v-for="(item, index) in dataList" :key="item.id"></listItem>

		</uni-list>

	</view>

</template>

<script>
	import {
		friendlyDate
	} from '@/common/util.js';

	import uList from '../../components/uni-list/uni-list.vue';
	import uCell from '../../components/uni-list-item/uni-list-item.vue';
	import listItem from '../../components/my-index/list-item.vue';

	export default {
		components: {
			uList,
			uCell,
			listItem
		},
		data() {
			return {
				dataList: [],
				isLoading: false
			}
		},
		created() {
			this.loadData();
		},
		methods: {
			loadData() {
				if (this.isLoading) {
					return;
				}

				this.isLoading = true;

				this.dataList.push("1");
			}
		}
	}
</script>

<style scoped>

</style>
