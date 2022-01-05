<template>
  <div class="">
    <van-cell-group>
      <van-cell  title="单元格">
          <template #default>
            <div @click="yulan">
              asdsads
            </div>
          </template>
      </van-cell>
    </van-cell-group>


      <div v-for="(item,index) in list" :key="index" @click="previewImg(index)"  >
        <span v-if="index===0">da</span>
      </div>
<!--<img src="../assets/x.png" @click="previewImg('../assets/x.png')" alt="">-->
  </div>
</template>

<script>
import { ImagePreview } from 'vant';
export default {
  name: 'HelloWorld',
  data() {
    return {
      msg: 'Welcome to Your Vue.js App',
      list:[
        'https://gitee.com/static/errors/images/logo.svg?t=158106664',
        'https://github.com/funinng/-/blob/main/5da0479e0001381f02940333.jpg?raw=true'
      ]
    }
  }, methods: {
    previewImg(index) {
      this.$hevueImgPreview({
        multiple: true,
        nowImgIndex: index,
        imgList: this.list
      })
    },yulan(){
      ImagePreview(['https://img01.yzcdn.cn/vant/apple-1.jpg']);
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="less" scoped>

</style>
