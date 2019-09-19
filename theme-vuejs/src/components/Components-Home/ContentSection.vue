<template>
  <div class="home-section">
    <div class="home-content-block">
      <div class="home-content-left">
        <h1 class="content-title">
          <h1 class="title-1">{{title1}}</h1>
          <h1 class="title-2">{{title2}}</h1>
          <h1 class="title-3">{{title3}}</h1>
        </h1>
        <h3>{{subTitle}}</h3>
        <span>{{content1}}</span><br/>
        <span>{{content2}}</span>
        <div class="list-content">
          {{listContent}}
          <li class="list1">{{list1}}</li>
          <li class="list2">{{list2}}</li>
          <li class="list3">{{list3}}</li>
          <li class="list4">{{list4}}</li>
          <li class="list5">{{list5}}</li>
        </div>
      </div>
      <div class="home-content-right"><img class="img-content" v-bind:src="imgUrl"></div>
    </div>
  </div>
</template>


<script>

export default {
  props: 
    [
      "title1", "title2", "title3", "subTitle", "content1", "content2", "listContent",
      "list1", "list2", "list3", "list4", "list5", "imgUrl"
    ]
};

</script>

<style scoped>

/* section 1 */

.section-1 .home-content-block{
  display: flex;
  align-items: center;
}

.section-1 .content-title{
  line-height: 0em;
}

.section-1 .home-section{
  margin-top: 5%;
}

.section-1 .home-content-left, .home-content-right{
  flex: 1;
}

.section-1 .title-1, .title-2, .title-3 {
    display: inline-block;
    font-size: 3rem;
    font-family: 'cloud-bold';
}

.section-1 .title-2{
  color:#00998d;
}

.section-1 .title-3{
  color:#ffca09;
}

.section-1 .list-content {
    margin-top: 7%;
}

.section-1 .list-content > li {
    margin-top: 1%;
}

.section-1 .img-content{
  width:100%;
}

/* section 1 */

/* section 2 */

.section-2 .home-content-block{
  display: flex;
  align-items: center;
  flex-direction: row-reverse;
}

.section-2 .content-title{
  line-height: 0em;
}

.section-2 .home-section{
  margin-top: 5%;
}

.section-2 .home-content-left, .home-content-right{
  flex: 1;
}

.section-2 .title-1, .title-2, .title-3 {
    display: inline-block;
    font-size: 3rem;
    font-family: 'cloud-bold';
}

.section-2 .title-1{
  color:#ffca09;
}

.section-2 .list-content {
    margin-top: 7%;
}

.section-2 .list-content > li {
    margin-top: 1%;
}

.section-2 .img-content{
  width:100%;
}

/* section 2 */

/* section 3 */

.section-3 .home-content-block{
  display: flex;
  align-items: center;
}

.section-3 .content-title{
  line-height: 0em;
}

.section-3 .home-section{
  margin-top: 5%;
}

.section-3 .home-content-left, .home-content-right{
  flex: 1;
}

.section-3 .title-1, .title-2, .title-3 {
    display: inline-block;
    font-size: 3rem;
    font-family: 'cloud-bold';
}

.section-3 .title-2{
  color:#00998d;
}

.section-3 .title-3{
  color:#ffca09;
}

.section-3 .list-content {
    margin-top: 7%;
}

.section-3 .list-content > li {
    margin-top: 1%;
}

.section-3 .img-content{
  width:100%;
}

/* section 3 */

</style>
