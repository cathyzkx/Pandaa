<template>
  <div class="caici-main">
    <div class="caici-word">
      <div>test</div>

    </div>
    <div class="caici-action">
      <el-button-group>
        <el-button icon="el-icon-arrow-left">上一页</el-button>
      </el-button-group>
      <el-button-group style="margin-right:30px; margin-left:30px">
        <el-button type="danger" icon="el-icon-error">{{noNum}}</el-button>
        <el-button type="success" icon="el-icon-success">{{yesNum}}</el-button>
      </el-button-group>
      <el-button-group>
        <el-button>下一页<i class="el-icon-arrow-right el-icon--right"></i></el-button>
      </el-button-group>
    </div>
    <div>
      <el-select v-model="value0" style="margin-right: 30px; margin-left:50px">
        <el-option
          v-for="item in options"
          :key="item.value"
          :label="item.label"
          :value="item.value">
        </el-option>
      </el-select>
      <el-button type="primary" @click="timeBegin">
        &nbsp;&nbsp;开始&nbsp;&nbsp;
        <i class="el-icon-caret-right"></i>
      </el-button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'AppMain',
  data () {
    return {
      yesNum: 0,
      noNum: 0,
      options: [{
        value: '60',
        label: '60s'
      }, {
        value: '90',
        label: '90s'
      }, {
        value: '120',
        label: '120s'
      }, {
        value: '180',
        label: '180s'
      }],
      value0: '60'
    }
  },
  methods: {
    timeBegin () {
      setTimeout(function () { alert('Hello') }, 3000)
    }
  }
}
</script>

<style>
.caici-main {
  display: flex;
  flex-direction: column;
  background: #ffffff;
}
.caici-word{
  line-height: 700px;
  width: 100%;
  font-size: 300px;
}
.caici-action{
  display: flex;
  align-items: center;
  justify-content: center;
  line-height: 100px;
  width: 100%;
  height:100px;
}
</style>
