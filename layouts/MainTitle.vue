<template>
    <div class="activity-layout">
      <!-- Section 1 ทำหน้าที่เหมือน br -->
      <div class="section1"></div>
  
      <!-- Section หลัก -->
      <div class="section">
        <motion :initial="{ opacity: 0, y: -20 }" :animate="{ opacity: 1, y: 0 }" transition="0.8s">
          <h1 class="main-title">Activity 6.1</h1>
        </motion>
      </div>
  
      <!-- Content Box -->
      <div class="content-box">
        <motion :initial="{ opacity: 0, y: 50 }" :animate="{ opacity: 1, y: 0 }" transition="1.2s">
          <h2 class="description-title">
            <span class="highlight-content">
              การประเมินความสุกของพวงกล้วยเพื่อความพร้อมสำหรับการเก็บเกี่ยวโดยใช้ Image Processing
            </span>
          </h2>
        </motion>
      </div>
    </div>
  </template>
  
  <style scoped>
  /* Activity Layout */
  .activity-layout {
    background-image: url('/assets/images/banaa.jpeg');
    background-color: rgba(0, 0, 0, 0.4);
    /* Add a semi-transparent overlay */
    background-size: cover;
    background-position: center;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
  }
  
  /* Section1: ใช้แทน br */
  .section1 {
    height: 90px; /* ปรับความสูงตามที่ต้องการ */
    width: 100%; /* ให้เต็มหน้าจอ */
    background-color: transparent; /* โปร่งใส */
  }
  
  /* Section */
  .section {
    margin-bottom: 20px; /* ระยะห่างระหว่าง section */
    background-color: rgba(0, 0, 0, 0.2); /* Semi-transparent box */
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1); /* Optional shadow */
    width: 60%; /* กำหนดความกว้างเป็น 90% ของหน้าจอ */
    max-width: 1200px; /* จำกัดความกว้างสูงสุด */
    padding: 20px; /* เพิ่มพื้นที่ภายในกล่อง */
    border-radius: 10px; /* มุมมน */
  }
  
  
  /* Main Title */
  .main-title {
    color: #fff;
    font-size: 3rem;
    margin-bottom: 2rem;
    text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.6);
  }
  
  /* Content Box */
  .content-box {
    width: 90%;
    text-align: center;
    padding: 30px;
    border: 3px solid #fff;
    border-radius: 15px;
    background-color: rgba(0, 0, 0, 0.7);
    /* Semi-transparent box */
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
    /* Optional shadow */
    overflow-y: auto;
    /* เพิ่มการเลื่อน */
    max-height: 90vh;
    /* จำกัดความสูง */
  }
  
  /* Description Title */
  .description-title {
    color: #fff;
    font-size: 1.8rem;
  }
  
  /* Highlight Content */
  .highlight-content {
    color: lime;
  }
  </style>
  