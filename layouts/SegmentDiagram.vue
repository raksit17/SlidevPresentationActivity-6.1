<template>
    <div class="green-layout">
      <div class="circle-diagram">
        <div class="center-circle">
          <h2>ความรู้ที่ต้องใช้</h2>
        </div>
        <!-- Segments -->
        <div class="segment segment-1">
          <span>1. ด้าน Image Processing</span>
        </div>
        <div class="segment segment-2">
          <span>2. ด้าน Machine Learning</span>
        </div>
        <div class="segment segment-3">
          <span>3. ด้านเกษตรศาสตร์</span>
        </div>
      </div>
    </div>
  </template>
  
  <style scoped>
  /* พื้นหลัง */
  .green-layout {
    background-image: url('/assets/images/banana-01.jpg'); /* พื้นหลัง */
    background-size: cover;
    background-position: center;
    color: white;
    height: 100vh; /* ครอบคลุมเต็มหน้าจอ */
    width: 100%;
    display: flex;
    justify-content: center; /* จัดกึ่งกลางแนวนอน */
    align-items: center; /* จัดกึ่งกลางแนวตั้ง */
    text-align: center;
    padding: 20px;
    box-sizing: border-box;
    
  }
  
  /* Circle Diagram */
  .circle-diagram {
    width: 600px; /* ขยายขนาด */
    height: 600px;
    margin: 0 auto;
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
    background: rgba(0, 0, 0, 0.2); /* พื้นหลังโปร่งแสง */
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
   
  }
  
  /* Center Circle */
  .center-circle {
    position: absolute;
    width: 230px;
    height: 230px;
    background: rgba(24, 65, 201, 0.9); /* สีขาวโปร่งแสง */
    color: #ffffff; /* ตัวอักษรสีขาว */
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    font-size: 18px;
    font-weight: bold;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.3);
    top: 50%; 
    text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5);
    font-size: 19px;
  }
  
  /* Segments */
  .segment {
    position: absolute;
    width: 220px; /* ขยายขนาดกล่อง */
    height: 220px;
    background: rgba(255, 255, 255, 0.7); /* สีพื้นหลังโปร่งแสง */
    color: black;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    border-radius: 50%;
    font-size: 16px;
    font-weight: bold;
    padding: 20px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    border: 2px solid rgba(0, 0, 0, 0.1);
    top: 20%; 

  }
  
  /* Specific Segment Positions */
  .segment-1 {
    top: 20%; /* วางด้านบน */
    left: 50%;
    transform: translate(-50%, -50%);
    background: rgba(103, 187, 121, 0.9); /* สีเขียวธรรมชาติ */
    color: #ffffff; /* ตัวอักษรสีขาว */
    text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5);
    font-size: 19px;
  }
  .segment-2 {
    bottom: 15%; /* วางซ้ายล่าง */
    left: 15%;
    transform: translate(-50%, 50%);
    background: rgba(229, 176, 76, 0.9); /* สีส้ม */
    color: #ffffff; /* ตัวอักษรสีขาว */
    text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5);
    font-size: 19px;
  }
  .segment-3 {
    bottom: 15%; /* วางขวาล่าง */
    right: 15%;
    transform: translate(50%, 50%);
    background: rgba(207, 81, 76, 0.9); /* สีแดงธรรมชาติ */
    color: #ffffff; /* ตัวอักษรสีขาว */
    text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5);
    font-size: 19px;
  }
  </style>
  