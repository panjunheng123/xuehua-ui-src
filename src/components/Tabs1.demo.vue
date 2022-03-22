<demo>
基础用法
</demo>
<template>
  <Tabs v-model:selected="x">
    <Tab title="吃饭">吃饭</Tab>
    <Tab title="睡觉">睡觉</Tab>
    <Tab title="打游戏">打游戏</Tab>
  </Tabs>
</template>

<script lang="ts">
import Tabs from '../lib/Tabs.vue';
import Tab from '../lib/Tab.vue';
import {
  ref
} from 'vue';

export default {
  components: {
    Tabs,
    Tab
  },
  setup() {
    const x = ref('打游戏');
    return {
      x
    };
  }
};
</script>