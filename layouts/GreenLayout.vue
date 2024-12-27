<template>
  <div class="green-layout">
    <header class="layout-header">
      <h1 class="gradient-title">{{ frontmatter.title }}</h1>
    </header>
    <main class="layout-content">
      <div class="content-row">
        <!-- Box 1 -->
        <div class="content-box">
          <h1 class="sub-title" >ปัญหาในการประเมินความสุกของพวงกล้วย</h1>
          <slot name="box1" />
        </div>
        <!-- Box 2 -->
        <div class="content-box">
          <h1 class="sub-title" >ผลกระทบ</h1>
          <slot name="box2" />
        </div>
      </div>
    </main>
    <footer class="layout-footer">
      <!-- <p>Banana Ripeness Detection | Powered by Slidev</p> -->
    </footer>
  </div>
</template>
  
  <script setup>
  defineProps(['frontmatter']); // รับค่า Front Matter
  </script>
  
  <style scoped>
  .green-layout {
    background-image: url('/assets/images/banana-01.jpg'); /* พื้นหลัง */
    background-size: cover;
    background-position: center;
    color: white;
    height: 100%;
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
    text-align: center;
  }
  .sub-title {
    background-color: rgb(255, 255, 255);
    background-image: linear-gradient(
      45deg,
      rgba(113, 255, 100, 1) 0%, /* สีเขียวสว่าง */
      rgba(30, 215, 88, 1) 100% /* สีเขียวเข้ม */
    );
    background-size: 100%;
    -webkit-background-clip: text;
    -moz-background-clip: text;
    -webkit-text-fill-color: transparent;
    -moz-text-fill-color: transparent;
    font-weight: bold;
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.7); /* เงาสีดำแบบโปร่ง */
    border-bottom: 3px solid #00ff80; /* เส้นขีดล่างสีเขียวอ่อน */
    padding-bottom: 5px;
    font-size: 1.2rem;
  }
  
  
  .layout-header {
    background-color: rgba(0, 0, 0, 0.8); /* โปร่งแสง */
    width: 100%;
    padding: 8px 0;
  }
  
  .gradient-title {
    font-size: 2.5rem;
    font-weight: bold;
    background: linear-gradient(90deg, #7fa914, #08fa65); /* สีข้อความ */
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin: 0;
  }
  
  .layout-content {
    flex: 1;
    display: flex;
    flex-direction: column;
    justify-content: space-around; /* จัดระยะห่าง */
    align-items: center;
    width: 100%;
  }
  .content-row {
    display: flex; /* ใช้ Flexbox */
    justify-content: space-between; /* กล่องอยู่ซ้ายขวา */
    gap: 20px; /* ระยะห่างระหว่างกล่อง */
    width: 90%; /* กำหนดความกว้างรวม */
    max-width: 1200px; /* จำกัดความกว้างสูงสุด */
  }
  .content-box {
    background-color: rgba(0, 0, 0, 0.9); /* พื้นหลังโปร่งแสง */
    border: 2px solid #ffe45e; /* สีกรอบ */
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    max-width: 800px;
    color: white;
    font-size: 1.5rem;
    line-height: 2; /* ระยะห่างระหว่างบรรทัด */
    text-align: left;
    width: 80%;
  }
  </style>
  