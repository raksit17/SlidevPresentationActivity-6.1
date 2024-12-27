<template>
  <div class="green-layout">
    <header class="layout-header">
      <h1 class="gradient-title">ความรู้ที่ต้องใช้  ด้านเกษตรศาสตร์</h1>
    </header>
    <main class="layout-content">
      <div class="content-row">
        <!-- กล่องเนื้อหา 1 -->
        <div class="content-box">
          <h2 class="sub-title">เกณฑ์การวัดความสุกของกล้วย</h2>
          <ul>
            <li>☘️ ศึกษาความสัมพันธ์ระหว่างสีเปลือกและระดับความสุก เช่น เขียว (ไม่สุก), เหลือง (สุกเต็มที่)</li>
          </ul>
        </div>
        <!-- กล่องเนื้อหา 2 -->
        <div class="content-box">
          <h2 class="sub-title">ลักษณะและการเติบโตของพวงกล้วย</h2>
          <ul>
            <li>☘️ วิเคราะห์ระยะการพัฒนาของพวงกล้วย เช่น ระยะเริ่มเปลี่ยนสี หรือขนาดผลที่เหมาะสม</li>
          </ul>
        </div>
      </div>
      <div class="content-row">
        <!-- กล่องเนื้อหา 3 -->
        <div class="content-box">
          <h2 class="sub-title">ผลกระทบจากสภาพแวดล้อม</h2>
          <ul>
            <li>☘️ ศึกษาผลกระทบจากแสงแดด ความชื้น และอุณหภูมิต่อการเปลี่ยนแปลงของสีและความสุก</li>
          </ul>
        </div>
      </div>
    </main>
  </div>
</template>

<script setup>
// ไม่มี JavaScript Logic ในที่นี้
</script>

<style scoped>
/* พื้นหลัง */
.green-layout {
  background-image: url('/assets/images/banana-01.jpg'); /* พื้นหลัง */
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  color: white;
  min-height: 100vh; /* ครอบคลุมหน้าจอ */
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  text-align: center;
  padding: 20px; /* เพิ่มระยะห่างรอบเนื้อหา */
  box-sizing: border-box; /* ให้ padding รวมอยู่ในขนาด */
}

/* หัวข้อใหญ่ */
.layout-header {
  background-color: rgba(0, 0, 0, 0.8); /* โปร่งแสง */
  width: 100%;
  padding: 0px 0;
}

.gradient-title {
  font-size: 2.5rem;
  font-weight: bold;
  background: linear-gradient(90deg, #7fa914, #08fa65); /* สีข้อความ */
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  margin: 0;
}

/* พื้นที่เนื้อหา */
.layout-content {
  flex: 1;
  display: flex;
  flex-direction: column;
  justify-content: flex-start; /* เลื่อนการจัดกล่องไปด้านบน */
  align-items: center;
  width: 100%;
  gap: 20px; /* เพิ่มระยะห่างระหว่างแถว */
}


.content-row {
  display: flex;
  justify-content: space-evenly;
  flex-wrap: wrap; /* ให้ย้ายไปบรรทัดใหม่เมื่อพื้นที่ไม่พอ */
  gap: 10px;
  width: 100%;
  max-width: 1200px;
  margin: 0 auto;
}

/* กล่องเนื้อหา */
.content-box {
  background-color: rgba(0, 0, 0, 0.85); /* สีพื้นหลังเข้มขึ้น */
  border: 2px solid #00ff80; /* เปลี่ยนสีกรอบเป็นสีเขียวสว่าง */
  padding: 23px; /* เพิ่มระยะห่างภายใน */
  border-radius: 12px; /* เพิ่มขอบมน */
  box-shadow: 0 6px 12px rgba(0, 0, 0, 0.4); /* เพิ่มเงาเพื่อความลึก */
  color: #e5ffe5; /* สีข้อความ */
  font-size: 1.1rem; /* ขนาดข้อความ */
  line-height: 1.8; /* ระยะห่างระหว่างบรรทัด */
  text-align: left; /* ชิดซ้าย */
  flex: 1; /* ให้กล่องขยายตามพื้นที่ */
  min-width: 200px; /* กำหนดความกว้างขั้นต่ำ */
  max-width: 500px; /* จำกัดความกว้างสูงสุด */
  margin: 20px; /* ระยะห่างระหว่างกล่อง */
  display: flex;
  flex-direction: column;
  align-items: flex-start;
}

/* หัวข้อย่อย */
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
  text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.7); /* เงาสีดำ */
  border-bottom: 3px solid #00ff80; /* เส้นขีดล่าง */
  padding-bottom: 5px;
  font-size: 1.1rem;
}

/* รองรับหน้าจอเล็ก */
@media (max-width: 768px) {
  .content-box {
    font-size: 1rem; /* ลดขนาดตัวอักษร */
    padding: 15px; /* ลดระยะห่างภายใน */
  }

  .content-row {
    flex-direction: column; /* จัดกล่องเป็นคอลัมน์ */
    align-items: center;
  }
}
</style>
