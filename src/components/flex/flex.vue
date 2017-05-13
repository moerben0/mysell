<template>
  <div class="message">
    <div class="line"></div>
    <div class="text">{{m[index]}}</div>
    <div class="line"></div>
  </div>
</template>

<script type="text/ecmascript-6">
    export default{
      props: {
        index: {
            type: Number
        }
      },
      data() {
        return {
            m: ['优惠信息', '商家公告']
        };
      }
    };
</script>

<style lang="stylus" rel="stylesheet/stylus">
  .message
    display: flex
    width: 80%
    margin: 28px auto 24px auto
    .line
      flex: 1
      position: relative
      top: -6px
      border-bottom: 1px solid rgba(255, 255, 255, 0.2)
    .text
      padding: 0 12px
      font-size: 14px
</style>
