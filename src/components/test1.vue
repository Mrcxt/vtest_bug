<!--
 * @LastEditTime: 2019-11-27 15:08:09
 * @Description: 
 * @Date: 2019-11-27 11:46:51
 * @Author: @虾哔哔
 -->
<template>
  <div>
    {{ test() }}
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  tag: null,
  methods: {
    test() {
      console.log("object");

      /*----------  添加上下面这段代码之后，就会被执行2次  ----------*/
      //   if (!this.tag) {
      //     this.tag = 1; //关键点，更改了 this.tag 的状态
      //   }
      /*----------    ----------*/
      let aaa = this.tag;
      this.tag = 1; // 关键点，如果不用if包裹，那么只会执行一次
    }
  }
};
</script>

<style lang="less" scoped></style>
