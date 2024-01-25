<template>
  <div class="topbar">
    <div class="logo"><span class="infinity">Infinity</span><span class="up">Up</span></div>
    <div class="menu"><div class="menu-icon-container" @click="toggleMenu"><Icon class="icon" name="mdi:menu" /></div></div>
  </div>
</template>

<script setup>
const { menuVisible, toggleMenu } = useGlobalState();
</script>

<style lang="scss" scoped>

*{
  color:$text-primary;
}
.menu-icon-container:hover{
  cursor:pointer;
}
.icon{
  font-size:28px;
}
.logo{
font-family: Inter;
font-size: 20px;
font-style: normal;
line-height: normal; 
}
.infinity{
  font-weight: 700;
}
.up{
  font-weight: 400;
}

.topbar{
background-color: $primary;
min-width:100%;
display: flex;
height: 56px;
padding: 10px 16px;
justify-content: space-between;
align-items: center;
flex-shrink: 0;
}

</style>