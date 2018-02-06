<template>
  <div class="hello">
    <div class="page-content container-fluid">
      <!--7777-->
      <div class="SB col-sm-12">
        <div class="SBTitle col-sm-12">
          <span class="col-sm-2">筛选条件</span>
          <span class="col-sm-1 pull-right">
            <button type="button" class="btn btn-default btn-sm">重置</button>
          </span>
          <span class="col-sm-1 pull-right">
            <button type="button" class="btn btn-default btn-sm">查询</button>
          </span>
        </div>
        <div class="col-sm-12">
          <div class="col-sm-1 text-right">产品：</div>
          <div class=" col-sm-4">
            <select class="form-control" :disabled="produceChooseD">
              <option value="1">行用卡偿贷1</option>
              <option value="2">行用卡偿贷2</option>
            </select>
          </div>
        </div>
        <div class="row">
          <div class="col-md-9" >.col-md-9 .col-md-push-3</div>
          <div class="col-md-3" >.col-md-3 .col-md-pull-9</div>
        </div>
      </div>

    </div>
  </div>
</template>

<script>
export default {
  name: 'unitTest',
  data:function() {
    var data = {'produceChooseD': false}
    return data
  },
  mounted: function () {

  },
  methods: {
    chooseM: function () {
      clearInterval( this.T1)
    },

  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
</style>
<style lang="scss" scoped >
  .hello{
    max-width: 1400px;
    min-width: 1000px;
  }
</style>
