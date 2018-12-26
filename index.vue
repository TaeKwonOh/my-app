<template>
  <div>
    <h3>그리드 컴포넌트 분리 예제</h3>
    <form id="search">
      Search
      <input name="query" v-model="searchQuery">
    </form>
    <grid-temp :data="gridData" :columns="gridColumns" :filter-key="searchQuery"></grid-temp>
    <h3>트리 컴포넌트 분리 예제</h3>
    <TreeTemp :model="treeData"></TreeTemp>
  </div>
</template>

<script>
import GridTemp from "./GridTemp";
import TreeTemp from "./TreeTemp";
export default {
  data: function() {
    return {
      searchQuery: "",
      gridColumns: [
        "LISTNUM",
        "CDLOGINNM",
        "CDLOGINIDK",
        "CDSTATUS",
        "CDORGNAME",
        "CDNAME",
        "UPPERAUTHNAME",
        "AUTHGROUPNAME",
        "INSERTDATE",
        "CDEXPDATE"
      ],
      gridData: [
        {
          LISTNUM: 1,
          CDLOGINNM: "부산지방경찰청 운영자",
          CDLOGINIDK: "operBU00!",
          CDSTATUS: "사용중",
          CDORGNAME: "부산지방경찰청(old)",
          CDNAME: "<NULL>",
          UPPERAUTHNAME: "<NULL>",
          AUTHGROUPNAME: "<NULL>",
          INSERTDATE: "2016.04.20 13:48:19",
          CDEXPDATE: "99991231"
        },
        {
          LISTNUM: 2,
          CDLOGINNM: "부산지방경찰청 운영자",
          CDLOGINIDK: "operBU00!",
          CDSTATUS: "사용중",
          CDORGNAME: "부산지방경찰청(old)",
          CDNAME: "<NULL>",
          UPPERAUTHNAME: "<NULL>",
          AUTHGROUPNAME: "<NULL>",
          INSERTDATE: "2016.04.20 13:48:19",
          CDEXPDATE: "99991231"
        },
        {
          LISTNUM: 3,
          CDLOGINNM: "부산지방경찰청 운영자",
          CDLOGINIDK: "operBU00!",
          CDSTATUS: "사용중",
          CDORGNAME: "부산지방경찰청(old)",
          CDNAME: "<NULL>",
          UPPERAUTHNAME: "<NULL>",
          AUTHGROUPNAME: "<NULL>",
          INSERTDATE: "2016.04.20 13:48:19",
          CDEXPDATE: "99991231"
        },
        {
          LISTNUM: 4,
          CDLOGINNM: "부산지방경찰청 운영자",
          CDLOGINIDK: "operBU00!",
          CDSTATUS: "사용중",
          CDORGNAME: "부산지방경찰청(old)",
          CDNAME: "<NULL>",
          UPPERAUTHNAME: "<NULL>",
          AUTHGROUPNAME: "<NULL>",
          INSERTDATE: "2016.04.20 13:48:19",
          CDEXPDATE: "99991231"
        },
        {
          LISTNUM: 5,
          CDLOGINNM: "부산지방경찰청 운영자",
          CDLOGINIDK: "operBU00!",
          CDSTATUS: "사용중",
          CDORGNAME: "부산지방경찰청(old)",
          CDNAME: "<NULL>",
          UPPERAUTHNAME: "<NULL>",
          AUTHGROUPNAME: "<NULL>",
          INSERTDATE: "2016.04.20 13:48:19",
          CDEXPDATE: "99991231"
        },
        {
          LISTNUM: 6,
          CDLOGINNM: "부산지방경찰청 운영자",
          CDLOGINIDK: "operBU00!",
          CDSTATUS: "사용중",
          CDORGNAME: "부산지방경찰청(old)",
          CDNAME: "<NULL>",
          UPPERAUTHNAME: "<NULL>",
          AUTHGROUPNAME: "<NULL>",
          INSERTDATE: "2016.04.20 13:48:19",
          CDEXPDATE: "99991231"
        },
        {
          LISTNUM: 7,
          CDLOGINNM: "부산지방경찰청 운영자",
          CDLOGINIDK: "operBU00!",
          CDSTATUS: "사용중",
          CDORGNAME: "부산지방경찰청(old)",
          CDNAME: "<NULL>",
          UPPERAUTHNAME: "<NULL>",
          AUTHGROUPNAME: "<NULL>",
          INSERTDATE: "2016.04.20 13:48:19",
          CDEXPDATE: "99991231"
        },
        {
          LISTNUM: 8,
          CDLOGINNM: "부산지방경찰청 운영자",
          CDLOGINIDK: "operBU00!",
          CDSTATUS: "사용중",
          CDORGNAME: "부산지방경찰청(old)",
          CDNAME: "<NULL>",
          UPPERAUTHNAME: "<NULL>",
          AUTHGROUPNAME: "<NULL>",
          INSERTDATE: "2016.04.20 13:48:19",
          CDEXPDATE: "99991231"
        },
        {
          LISTNUM: 9,
          CDLOGINNM: "부산지방경찰청 운영자",
          CDLOGINIDK: "operBU00!",
          CDSTATUS: "사용중",
          CDORGNAME: "부산지방경찰청(old)",
          CDNAME: "<NULL>",
          UPPERAUTHNAME: "<NULL>",
          AUTHGROUPNAME: "<NULL>",
          INSERTDATE: "2016.04.20 13:48:19",
          CDEXPDATE: "99991231"
        },
        {
          LISTNUM: 10,
          CDLOGINNM: "부산지방경찰청 운영자",
          CDLOGINIDK: "operBU00!",
          CDSTATUS: "사용중",
          CDORGNAME: "부산지방경찰청(old)",
          CDNAME: "<NULL>",
          UPPERAUTHNAME: "<NULL>",
          AUTHGROUPNAME: "<NULL>",
          INSERTDATE: "2016.04.20 13:48:19",
          CDEXPDATE: "99991231"
        },
        {
          LISTNUM: 11,
          CDLOGINNM: "부산지방경찰청 운영자",
          CDLOGINIDK: "operBU00!",
          CDSTATUS: "사용중",
          CDORGNAME: "부산지방경찰청(old)",
          CDNAME: "<NULL>",
          UPPERAUTHNAME: "<NULL>",
          AUTHGROUPNAME: "<NULL>",
          INSERTDATE: "2016.04.20 13:48:19",
          CDEXPDATE: "99991231"
        }
      ],
      treeData: {
        name: "Todos-client",
        children: [
          { name: "assets", children: [{ name: "logo.png" }] },
          {
            name: "components",
            children: [
              { name: "GridTemp.vue" },
              { name: "HelloVorld.vue" },
              { name: "TestMenu.vue" },
              { name: "TreeTemp.vue" }
            ]
          },
          { name: "router", children: [{ name: "index.js" }] }
        ]
      }
    };
  },
  components: {
    GridTemp: GridTemp,
    TreeTemp: TreeTemp
  }
};
</script>

<style>
</style>
