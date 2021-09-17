<!--
 * @Author: Leo
 * @Date: 2021-09-16 17:06:56
 * @LastEditors: Leo
 * @LastEditTime: 2021-09-17 11:28:42
 * @Description: file content
-->
# 环境依赖
vue v2.6+
# 安装
npm i vue-telinput-pixus
# 使用示例
```js
<template>
  <div class="tel-container">
    <country-code-selector :countryCode.sync="value">
    </country-code-selector>
    <input type="text" v-model="value">
    <p>这是国际区号{{value}}</p>
  </div>
</template>

<script>
  import countryCodeSelector from 'vue-telinput-pixus'
  export default {
    name: 'VueTelInput',
    components: {
      countryCodeSelector
    },
    data () {
      return {
        // 这里是必填项。对应国家的国际区号，例如中国是86
        value: 86
      }
    }
  }
</script>

<style scoped>
  p {
    margin-left: 20px;
  }
</style>
```
