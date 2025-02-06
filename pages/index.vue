<template>
  <div class="box d-flex justify-content-center align-items-center">
    <div id="app" class="container">
      <div class="welcome-container">
        <div class="stars left-star">★</div>
        <div class="welcome-text">WELCOME</div>
        <div class="stars right-star">★</div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.box {
  height: 100vh;
  width: 100vw;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  background-image: url('/assets/img/latar.jpg');
  display: flex;
  justify-content: center;
  align-items: center;
  opacity: 0.6; /* Membuat gambar latar transparan 60% */
}

.container {
  height: 90vh; 
  width: 90vw; 
  display: flex;
  justify-content: center;
  align-items: center;
  font-family: "Times New Roman", Times, serif;
  border-radius: 10px;
  box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.2);
  box-sizing: border-box;
}

.welcome-container {
  display: flex;
  align-items: center;
  background: rgba(255, 255, 255, 0.8);
  padding: 20px 40px;
  border-radius: 10px;
  box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.2);
}

.welcome-text {
  font-size: 32px;
  font-weight: bold;
  margin: 0 10px;
}

.stars {
  color: red;
  font-size: 24px;
}

.left-star {
  margin-right: 10px;
}

.right-star {
  margin-left: 10px;
}

h1, h2 {
  margin: 0;
}
</style>

<script>
export default {
  name: "App",
};
</script>