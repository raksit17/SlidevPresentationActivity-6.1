<template>
    <div class="banana-leaf"></div>
  </template>
  
  <style scoped>
  .banana-leaf {
    width: 50px;
    height: 25px;
    background-color: #6b8e23; /* สีเขียวใบ */
    border-radius: 50% 50% 50% 0; /* รูปทรงใบ */
    transform: rotate(-30deg); /* เอียงใบ */
    box-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3); /* เงา */
    position: relative;
  }
  
  .banana-leaf::before {
    content: '';
    width: 50%;
    height: 50%;
    background-color: #9acd32; /* สีเขียวอ่อน */
    border-radius: 50%;
    position: absolute;
    top: 25%;
    left: 25%;
    z-index: 1;
  }
  
  .banana-leaf::after {
    content: '';
    width: 4px;
    height: 100%;
    background-color: #556b2f; /* เส้นกลางใบ */
    position: absolute;
    top: 0;
    left: 48%;
    z-index: 2;
  }
  </style>
  