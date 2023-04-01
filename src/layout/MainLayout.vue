<template>
  <main class="Main-layout">
    <Sidebar/>
    <div class="main-wrapper">
        <profile-menu/>
        <div class="main-router-content">
            <slot/>
        </div>
    </div>
    
  </main>
</template>

<script>
import Sidebar from './sidebar.vue';
import ProfileMenu from './profileMenu.vue';
export default {
    components:{
        Sidebar,
        ProfileMenu,
    }
}
</script>

<style>
.Main-layout{
    display: flex;
    height: 100vh;
    width: 100%;
}
.main-wrapper{
    flex-grow: 1;
}
</style>