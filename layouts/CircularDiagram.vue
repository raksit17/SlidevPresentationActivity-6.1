<template>
    <div class="green-layout">
      <div class="circular-diagram">
        <div class="diagram-center">
          <h2>วิธีการทำ</h2>
        </div>
        <!-- Segments -->
        <div class="diagram-segment segment-1">
          <div class="segment-content">
            <div class="emoji">📊</div>
            <h3>การรวบรวมข้อมูล</h3>
            <p>(Data Collection)</p>
          </div>
        </div>
        <div class="diagram-segment segment-2">
          <div class="segment-content">
            <div class="emoji">🖼️</div>
            <h3>การประมวลผลภาพ</h3>
            <p>(Image Preprocessing)</p>
          </div>
        </div>
        <div class="diagram-segment segment-3">
          <div class="segment-content">
            <div class="emoji">🎨</div>
            <h3>การวิเคราะห์สี</h3>
            <p>(Feature Extraction)</p>
          </div>
        </div>
        <div class="diagram-segment segment-4">
          <div class="segment-content">
            <div class="emoji">🤖</div>
            <h3>การฝึกโมเดล</h3>
            <p>(Machine Learning)</p>
          </div>
        </div>
        <div class="diagram-segment segment-5">
          <div class="segment-content">
            <div class="emoji">🔧</div>
            <h3>การทดสอบ</h3>
            <p>(Testing & Optimization)</p>
          </div>
        </div>
        <div class="diagram-segment segment-6">
          <div class="segment-content">
            <div class="emoji">🚀</div>
            <h3>การนำไปใช้งาน</h3>
            <p>(Deployment)</p>
          </div>
        </div>
      </div>
    </div>
  </template>
  
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
    justify-content: center;
    align-items: center;
    text-align: center;
  }
  
  .circular-diagram {
    position: relative;
    width: 600px;
    height: 600px;
    margin: 0 auto;
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
    background: rgba(125, 205, 140, 0.8); /* สีพื้นหลังโปร่งแสง */
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
  }
  
  .diagram-center {
    position: absolute;
    width: 150px;
    height: 150px;
    background: rgba(0, 115, 230, 0.9); /* สีพื้นหลังโปร่งแสง */
    color: white;
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    font-size: 18px;
    font-weight: bold;
    z-index: 10;
  }
  
  .diagram-segment {
    position: absolute;
    width: 200px;
    height: 200px;
    background: rgba(255, 255, 255, 0.9); /* โปร่งแสง */
    border-radius: 50%;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    transform-origin: center;
  }
  
  .segment-content {
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
  }
  
  .emoji {
    font-size: 36px; /* ขนาด Emoji */
    margin-bottom: 10px;
  }
  
  .segment-content h3 {
    font-size: 14px;
    font-weight: bold;
    margin: 0;
    color: #333;
  }
  
  .segment-content p {
    font-size: 12px;
    margin: 0;
    color: #666;
  }
  
  /* Positioning Segments */
  .segment-1 {
    top: 15%;
    left: 50%;
    transform: translate(-50%, -50%);
  }
  .segment-2 {
    top: 30%;
    left: 85%;
    transform: translate(-50%, -50%);
  }
  .segment-3 {
    top: 70%;
    left: 85%;
    transform: translate(-50%, -50%);
  }
  .segment-4 {
    top: 85%;
    left: 50%;
    transform: translate(-50%, -50%);
  }
  .segment-5 {
    top: 70%;
    left: 15%;
    transform: translate(-50%, -50%);
  }
  .segment-6 {
    top: 30%;
    left: 15%;
    transform: translate(-50%, -50%);
  }
  </style>
  