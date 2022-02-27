<style scoped>
section {
  height: 150px;
  background-color: #95db5e;
  margin: 0 5% 20px 5%;
  margin: 40px 0px;
}

div {
    margin: 40px 20px;
}
</style>

<template>
  <div class="container">
    <header-comp></header-comp>

    <section id="page1" data-role="page">
        <div class="content" data-role="content">컨텐츠</div>
    </section>

    <footer-comp></footer-comp>
  </div>
</template>

<script>
import Header from "./HeaderComp.vue";
import Footer from "./FooterComp.vue";

export default {
  data() {
    return {
      msg: "Hello VueJS",
    };
  },
  components: { // 변수명과 태그를 매핑해준다.  -- 소스를 먼저 결합한다.
    "header-comp": Header, //태그에 header 변수 추가
    "footer-comp": Footer, // 태그에 footer 변수 추가
  },
};
</script>
