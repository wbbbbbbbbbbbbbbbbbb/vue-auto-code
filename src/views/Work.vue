<template>
	<div class="workMain">
		<Row class-name="row" type="flex" align="middle" justify="center">
			<Card style="width:1200px">
				<p slot="title">工作区</p>
				<component :is="item" v-for="(item, index) in layout" :key="index"></component>
			</Card>
		</Row>
	</div>
</template>

<script>
import Text from '@/components/Text'

export default {
	data() {
		return {
			layout: [Text]
		}
	},
	components: {
		Text: () => import('@/components/Text'),
		Text1: Text,
		Text2: Text,
	},
	mounted() {},
	methods: {}
}
</script>

<style lang='less' scoped>
.workMain {
	height: 100%;
	padding: 30px 0;
}
</style>
