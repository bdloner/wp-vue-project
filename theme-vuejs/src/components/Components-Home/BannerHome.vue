<template>
  <div class="section-home-banner">
    <div class="home-banner-block">
      <div class="content-banner-left-block">
        <h1 class="title-concept">
          CREATE
          <br />INSPIRE
          <br />CONNECT
        </h1>
        <p>ทุกการสร้างสรรค์เกิดจากไอเดีย<br/>ของคุณกับผึ้งอย่างเราที่เข้าใจกัน</p>
        <p>“เพราะผึ้งรู้ว่าเกสรดอกไม้ชนิดไหน<br/>ดีที่สุดสำหรับคุณ”</p>
      </div>
      <div class="img-banner-right-block">
        <img
          class="img-banner-right"
          v-bind:src="'../vueproject/wp-content/uploads/2019/09/cover-front-1.svg'"
        />
      </div>
    </div>
  </div>
</template>

<style scoped>

.section-home-banner {
    position: relative;
    margin-left: 50%;
    width: 100vw;
    left: -50vw;
}

.home-banner-block {
    display: flex;
    align-items: center;
    padding: 0 9%;
    padding-bottom: 7%;
    height: 70vh;
    background-image: url(@~/vueproject/wp-content/uploads/2019/09/front-1.svg);
    background-position: bottom;
    background-size: cover;
}

.content-banner-left-block {
    flex: 1;
    padding-left:15%
}

.img-banner-right-block {
    flex: 1;
}

.img-banner-right{
    width:60%;
}

.title-concept{
    font-family: 'cloud-bold';
}

.img-banner-right-block {
    text-align: left;
}

</style>