<template>
  <div>
    <banner-home></banner-home>
    <content-section class="section-1"
      title1="Branding" 
      title2="&" 
      title3="Corporate Identity" 
      subTitle="สร้างแบรนด์ และอัตลักษณ์ที่สื่อถึงตัวตนคุณ" 
      content1="ไม่ว่าธุรกิจของคุณจะเป็นแบบไหน เราจะช่วยสร้างสรรค์แบรนด์ของคุณให้โดดเด่น มีเอกลักษณ์ ตั้งแต่การออกแบบโลโก้ ตัวอักษร 
      สีที่ใช้ ไอคอน ไปจนถึง mood & tone ที่จะใช้สื่อสารในงานกราฟิกต่างๆ เพื่อสื่อถึงตัวตนของธุรกิจคุณมากที่สุด"
      listContent="ผึ้งพร้อมเสิร์ฟ…"
      list1="Logo Design"
      list2="Fonts Usage"
      list3="Color scheme"
      list4="Icon / Symbol"
      list5="Key Visual"
      imgUrl="../vueproject/wp-content/uploads/2019/09/section-1-left.png"
      >
    </content-section>

    <content-section class="section-2"
      title1="Brand" 
      title2="Communication" 
      title3="" 
      subTitle="สื่อสารให้ชัด จัดให้ตรงกลุ่มเป้าหมาย" 
      content1="สื่อสารแบรนด์และธุรกิจของคุณ ผ่านสื่อต่างๆ ทุกช่องทาง โดยยึดเอกลักษณ์ของแบรนด์เป็นหลัก เพื่อให้การสื่อสารไปยังกลุ่มลูกค้าเป็นไปในทิศทางเดียวกัน"
      listContent="ผึ้งพร้อมเสิร์ฟ…"
      list1="Logo Design"
      list2="Fonts Usage"
      list3="Color scheme"
      list4="Icon / Symbol"
      list5="Key Visual"
      imgUrl="../vueproject/wp-content/uploads/2019/09/section-1-left.png"
      >
    </content-section>

    <content-section class="section-3"
      title1="Branding" 
      title2="" 
      title3="Corporate Identity" 
      subTitle="สร้างแบรนด์ และอัตลักษณ์ที่สื่อถึงตัวตนคุณ" 
      content1="test"
      listContent="ผึ้งพร้อมเสิร์ฟ…"
      list1="Logo Design"
      list2="Fonts Usage"
      list3="Color scheme"
      list4="Icon / Symbol"
      list5="Key Visual"
      imgUrl="../vueproject/wp-content/uploads/2019/09/section-1-left.png"
      >
    </content-section>
    <recent-posts-widget limit="5">Recent Posts</recent-posts-widget>
    <pages-widget limit="5">Pages</pages-widget>
  </div>
</template>

<script>
import RecentPostsWidget from "./widgets/RecentPosts.vue";
import PagesWidget from "./widgets/Pages.vue";
import BannerHome from "./Components-Home/BannerHome.vue";
import ContentSection from "./Components-Home/ContentSection.vue";

export default {

  components: {
    BannerHome,
    ContentSection,
    RecentPostsWidget,
    PagesWidget
  }
};

</script>
