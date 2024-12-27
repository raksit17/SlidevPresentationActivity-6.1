<template>
    <div class="green-layout">
      <div class="content-box">
        <h1>การฝึกโมเดล Machine Learning</h1>
        <div class="section">
          <h2 class="section-title"> โมเดลสำหรับการจำแนกความสุก</h2>
          <hr class="section-divider" />
          <ul>
            <li> <span class="icon">☘️</span>ใช้ ResNet  วิเคราะห์ลักษณะสีและ Texture ของพวงกล้วย</li>
            <li> <span class="icon">☘️</span>ใช้เทคนิค  Transfer Learning ในการฝึก</li>
            
          </ul>
        </div>
        <div class="section">
          <h2 class="section-title">โมเดลสำหรับการตรวจจับวัตถุ</h2>
          <hr class="section-divider" />
          <ul>
            <li> <span class="icon">☘️</span>ใช้ YOLOv8 ตรวจจับตำแหน่งพวงกล้วยในภาพ </li>
          </ul>
        </div>
        <div class="section">
          <h2 class="section-title">การเพิ่มข้อมูล (Data Augmentation):</h2>
          <hr class="section-divider" />
          <ul>
            <li> <span class="icon">☘️</span>หมุนภาพ (Rotation), สะท้อนภาพ (Flip), เปลี่ยนสี (Color Jitter), และครอบภาพ (Cropping)</li>
          </ul>
        </div>

      </div>
    </div>
  </template>
  
  <style scoped>
  .icon {
    margin-right: 10px;
    background: linear-gradient(90deg, #8fe114, #f4d03f);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }
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
    justify-content: flex-start; /* ให้เนื้อหาเริ่มจากบนสุด */
    align-items: center;
    text-align: left; /* ข้อความชิดซ้าย */
    padding: 20px; /* เพิ่มระยะห่างรอบเนื้อหา */
    box-sizing: border-box; /* ให้ padding รวมอยู่ในขนาด */
  }
  
  .content-box {
    background-color: rgba(0, 0, 0, 0.7); /* พื้นหลังโปร่งแสง */
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3); /* เพิ่มเงา */
    max-width: 800px;
    width: 100%;
    color: white;
    overflow-y: auto; /* เพิ่มการเลื่อน */
    max-height: 90vh; /* จำกัดความสูง */
  }
  
  h1 {
    font-size: 1.8rem;
    margin-bottom: 20px;
    text-align: center; /* หัวข้อใหญ่จัดกึ่งกลาง */
    color: #ffdf00; /* สีเน้นของหัวข้อใหญ่ */
  }
  
  .section-title {
    font-size: 1.1rem;
    color: #00ffcc; /* สีเน้นของหัวข้อย่อย */
    margin: 10px 0;
  }
  
  .section-divider {
    border: 0;
    border-top: 2px solid #ffffff; /* เส้นแบ่งหัวข้อ */
    margin: 10px 0 20px;
  }
  
  ul {
    margin: 0;
    padding-left: 20px;
  }
  
  ul ul {
    margin: 5px 0;
  }
  
  li {
    font-size: 0.9rem; /* ลดขนาดฟอนต์ */
    margin-bottom: 6px; /* ลดระยะห่างระหว่างรายการ */
    line-height: 1.4; /* ลดระยะห่างระหว่างบรรทัด */
  }
  </style>
  