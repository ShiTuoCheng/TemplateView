<template>
  <div class="header">
    <div class="logo" url="/views/template_2" target="_self"></div>

    <ul>
        <li class="active li_click" url="/views/template_2" target="_self">网站首页</li>
        <li @click="isShow =! isShow">图片展示
            <ul v-show="isShow" class="subNav">
                <li class="subNavItem" url="/views/template_2/projectDisplay.html" target="_self">案例展示</li>
                <li class="subNavItem" url="/views/template_2/productDisplay.html" target="_self">产品展示</li>
            </ul>
        </li>
        <li class="li_click" url="/views/template_2/newsCenter.html" target="_self">新闻列表
        </li>
        <li class="li_click" url="/views/template_2/about.html" target="_self">关于企业</li>
        <li class="li_click" url="/views/template_2/contactUs.html" target="_self">联系我们</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'header',
  data() {
      return{
          isShow: false
      }
  },

  methods: {

     
  }
}
</script>

<style scoped>
div.header {
  width: 1200px;
  margin: 0 auto;
}

ul {
  list-style-type: none;
  position: relative;
  float: right;
  padding: 0;
}

li {
  display: inline-block;;
  margin: 0 10px;
  cursor: pointer;
}

ul.subNav{
    display: block;
    position: absolute;
    top: 30px;
}

li.subNavItem{
    display: block;
    line-height: 24px;
    margin: 0;
}
</style>
