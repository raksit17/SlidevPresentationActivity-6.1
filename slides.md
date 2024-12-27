---
title: Activity 6.1
theme: seriph
background: /assets/images/banaa.jpeg
backgroundOverlay: rgba(0, 0, 0, 0.4)
backgroundSize: cover
backgroundPosition: center
transition: slide

---

# Activity 6.1

<div style="text-align: center; padding: 20px; border: 3px solid #fff; border-radius: 10px; background-color: rgba(0, 0, 0, 0.5);">
  <motion :initial="{ opacity: 0, y: 50 }" :animate="{ opacity: 1, y: 0 }" transition="0.8s">
    <h1 style="color: #fff; font-size: 2em; margin-bottom: 0.5em;"><span style="color: lime;">การประเมินความสุกของพวงกล้วยพื่อความพร้อมสำหรับการเก็บเกี่ยวโดยใช้ Image Processing</span></h1>
  </motion>
  <motion :initial="{ opacity: 0 }" :animate="{ opacity: 1 }" transition="1.2s">
    <!-- <p style="color: #ccc; font-size: 1.5em;">การประเมินความสุกของพวงกล้วยน้ำว้าในต้นเพื่อความพร้อมสำหรับการเก็บเกี่ยวโดยใช้ Image Processing</p> -->
  </motion>
</div>
---
layout: GreenLayout
title: ปัญหาที่สนใจ
components:
  - CustomList
---

<template #box1>
<CustomList :items="[{}, {}, {}]">
  <template #default="{ item, index }">
    <div v-if="index === 0">
      <strong style="background: linear-gradient(90deg, #c4e17f, #f7d26d); -webkit-background-clip: text; -webkit-text-fill-color: transparent;">
        ความแตกต่างของความสุกในพวงเดียวกัน
      </strong> 
      พวงกล้วยอาจมีผลที่สุกไม่เท่ากัน ทำให้ยากต่อการประเมิน
    </div>
    <div v-else-if="index === 1">
      <strong style="background: linear-gradient(90deg, #c4e17f, #f7d26d); -webkit-background-clip: text; -webkit-text-fill-color: transparent;">
        การสูญเสียผลผลิต
      </strong> 
      เก็บเกี่ยวก่อนหรือหลังช่วงเวลาที่เหมาะสม ส่งผลต่อคุณภาพของผลผลิต
    </div>
    <div v-else>
      <strong style="background: linear-gradient(90deg, #c4e17f, #f7d26d); -webkit-background-clip: text; -webkit-text-fill-color: transparent;">
        ข้อจำกัดในสวนขนาดใหญ่
      </strong> 
      การประเมินด้วยแรงงานใช้เวลานาน
    </div>
  </template>
</CustomList>
</template>

<template #box2>
<CustomList :items="[{}, {}]">
  <template #default="{ item, index }">
    <div v-if="index === 0">
      การเก็บเกี่ยวล่าช้า
    </div>
    <div v-else-if="index === 1">
      คุณภาพผลผลิตลดลง
    </div>
  </template>
</CustomList>
</template>


---
layout: Slides3
title: เป้าหมายหรือวัตถุประสงค์
components:
  - CustomListSlide3
---

<template #box1>
<CustomListSlide3 :items="[{}, {}]">
  <template #default="{ item, index }">
    <div v-if="index === 0">
      <strong style="background: linear-gradient(90deg, #c4e17f, #f7d26d); -webkit-background-clip: text; -webkit-text-fill-color: transparent;">
        พัฒนาระบบประเมินความสุกของพวงกล้วย
      </strong> 
      สร้างระบบที่ใช้ Image Processing และ Machine Learning ในการประเมินความสุก และ รองรับการทำงานแบบอัตโนมัติและเรียลไทม์
    </div>
    <div v-else-if="index === 1">
      <strong style="background: linear-gradient(90deg, #c4e17f, #f7d26d); -webkit-background-clip: text; -webkit-text-fill-color: transparent;">
        สนับสนุนการจัดการผลผลิต
      </strong> 
      ลดความคลาดเคลื่อนที่เกิดจากสายตามนุษย์และลดการสูญเสียผลผลิตจากการเก็บเกี่ยวในช่วงเวลาที่ไม่เหมาะสม
    </div>
  </template>
</CustomListSlide3>
</template>

---
layout: SegmentDiagram
title: เป้าหมายหรือวัตถุประสงค์
---

---
layout: Slides4
title: เป้าหมายหรือวัตถุประสงค์
---
---
layout: Slides5
title: เป้าหมายหรือวัตถุประสงค์
---
---
layout: Slides6
title: เป้าหมายหรือวัตถุประสงค์
---
---
layout: CircularDiagram
title: เป้าหมายหรือวัตถุประสงค์
---
---
layout: Sldes7
title: เป้าหมายหรือวัตถุประสงค์
---
---
layout: Sldes8
title: เป้าหมายหรือวัตถุประสงค์
---
---
layout: Sldes9
title: เป้าหมายหรือวัตถุประสงค์
---
---
layout: Sldes10
title: เป้าหมายหรือวัตถุประสงค์
---------

---
---
layout: Sldes11
title: เป้าหมายหรือวัตถุประสงค์

---
---
layout: Sldes12
title: เป้าหมายหรือวัตถุประสงค์
---------

