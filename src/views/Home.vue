<template>
	<div class="homeMain">
		<Work/>
    <Plugin class="plugin"/>
	</div>
</template>

<script>
import Plugin from './Plugin'
import Work from './Work'

export default {
  components: {
    'Plugin': Plugin,
    'Work': Work
  }
}
</script>

<style lang="less" scoped>
.homeMain {
	height: 100%;
  position: relative;

  .plugin {
    position: absolute;
    top: 30px;
    right: 30px;
  }
}
</style>
