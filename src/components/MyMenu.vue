<template>
  <div>
    <el-menu class="menu" :default-active="activeIndex" mode="horizontal" background-color="#191C24" text-color="#fff" active-text-color="red" menu-trigger="click">
      <el-menu-item index="1"><input src="text" /></el-menu-item>
      <el-submenu index="2">
        <template slot="title">Message</template>
         <el-menu-item index="2-1">
           <div class="childmenu">
             <p>Jhon send you a message</p>
             <span>15 minutes ago</span>
           </div>
         </el-menu-item>
         <el-menu-item index="2-2">
           <div class="childmenu">
             <p>Jhon send you a message</p>
             <span>15 minutes ago</span>
           </div>
          </el-menu-item>
         <el-menu-item index="2-3">
           <div class="childmenu">
             <p>Jhon send you a message</p>
             <span>15 minutes ago</span>
           </div>
          </el-menu-item>
      </el-submenu>
      <el-menu-item index="3">Notificatin</el-menu-item>
      <el-menu-item index="4">John Doe</el-menu-item>
     
    </el-menu>
    <!-- 垂直 -->

    <el-menu
        text-color="#fff" 
        background-color="#191C24"
        class="my-menu"
        default-active="1">
      <el-menu-item index="1">Dashboard</el-menu-item>
      <el-submenu index="2">
        <template slot="title">Elements</template>
        <el-menu-item index="2-1">Buttons</el-menu-item>
        <el-menu-item index="2-2">Typography</el-menu-item>
        <el-menu-item index="2-3">Other Elements</el-menu-item>
      </el-submenu>
      <el-menu-item index="3">Widgets</el-menu-item>
      <el-menu-item index="4">Form</el-menu-item>
      <el-menu-item index="5">Tables</el-menu-item>
      <el-menu-item index="6">Charts</el-menu-item>
      <el-submenu index="7">
        <template slot="title">Pages</template>
        <el-menu-item index="7-1">Sign In</el-menu-item>
        <el-menu-item index="7-2">Sign Up</el-menu-item>
        <el-menu-item index="7-3">404 Error</el-menu-item>
        <el-menu-item index="7-4">Blank Page</el-menu-item>
      </el-submenu>
    </el-menu>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        activeIndex: '3',
      }
    },
  }
</script>

<style scoped>

.my-menu {
    width: 10vw;
    height: 100vh;
}
.childmenu{
  line-height: 10px;
  display: block;
  
}
span{
    border-bottom: 1px solid white;
  }
</style>