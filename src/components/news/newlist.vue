<template>
  <div class="newlist">
    <!-- <ul>
      <li v-for="(item, index) in newlist" :key="index">id:{{item.id}}----------name:{{item.name}}</li>
    </ul>-->
    <ul class="mui-table-view">
      <li class="mui-table-view-cell mui-media">
        <router-link :to="'/home/newlist/'+1">
          <img
            class="mui-media-object mui-pull-left"
            src="/static/image/1.jpg"
          />
          <div class="mui-media-body">
            幸福 {{newlist.a|dataFormate}}
            <p class="mui-ellipsis">能和心爱的人一起睡觉，是件幸福的事情；可是，打呼噜怎么办？</p>
          </div>
        </router-link>
      </li>
      <li class="mui-table-view-cell mui-media">
        <router-link to="/home/newlist/2">
          <img
            class="mui-media-object mui-pull-left"
            src="/static/image/2.jpg"
          />
          <div class="mui-media-body">
            木屋
            <p class="mui-ellipsis">想要这样一间小木屋，夏天挫冰吃瓜，冬天围炉取暖.</p>
          </div>
        </router-link>
      </li>
      <li class="mui-table-view-cell mui-media">
        <router-link to="/home/newlist/3">
          <img
            class="mui-media-object mui-pull-left"
            src="/static/image/3.jpg"
          />
          <div class="mui-media-body">
            CBD
            <p class="mui-ellipsis">烤炉模式的城，到黄昏，如同打翻的调色盘一般.</p>
          </div>
        </router-link>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "newlist",
  data() {
    return {
      newlist: [
        { id: 1, name: "PDD" },
        { id: 2, name: "马飞飞" },
        { id: 3, name: "卢本伟" },
        { a: new Date() }
      ]
    };
  }
};
</script>

<style>
ul li {
  list-style-type: none;
  width: 100%;
  padding: 10px;
  border: dashed 1px solid;
}
</style>