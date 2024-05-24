<template>
  <div class="container">
    <div class="header">
      <img src="../assets/signlanguage.jpg" alt="signlanguage"/>
      <h1>Xin chào</h1>
      <p>Về chúng tôi</p>
    </div>
    <div class="content">
      <div class="section">
        <h3>TUNU là web học thủ ngữ bằng việc chơi game</h3>
        <p>Background</p>
        <p>Alipaam lorem ante, dapilen in, vivrera quis, feugiat a, tellus.
        ru Phasellus viverra nulla ut martus varius laoreet. Quisque rut...</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'AboutMe',
};
</script>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 20px;
}

.header {
  text-align: center;
  margin-bottom: 20px;
}

.content {
  width: 600px;
}

.section {
  margin-bottom: 20px;
}
</style>
