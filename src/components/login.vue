<script lang="ts"setup>
import { ref } from 'vue'
const input = ref('')
const password = ref('')
</script>


<template>
    <el-card style="max-width: 480px;display: grid; place-items: center;">
      <template #header>
        <div class="card-header">
          <span>用户登录</span>
        </div>
      </template>
      <el-form :model="form" label-width="auto" style="max-width: 600px">
        <el-form-item label="用户名">
            <el-input v-model="input" style="width: 240px" placeholder="" />
        </el-form-item>
        <el-form-item label="密码">
            <el-input v-model="password" style="width: 240px" type="password" placeholder="" show-password/>
        </el-form-item>
        <el-form-item>
            <el-button>重置</el-button>
            <el-button type="primary">提交</el-button>
        </el-form-item>
      </el-form>
    </el-card>
  </template>
  
<style scoped>
element.style{
    margin-left: 80px;
}

</style>