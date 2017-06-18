<template>
  <div class="welcomeMan">
    <header>
      <div class="header-top">

      </div>
      <div class="header-middle">

      </div>
      <div class="header-bottom">
        <div class="middle">
          <h2>邓婧雯</h2>
          <p>湖南岳阳</p>
          <div class="myself">
          </div>
        </div>
      </div>
    </header>

    <footer>
      <p class="what">me</p>
      <p class="what-text">来看打了卡我拿到了卡我恨你打了卡很无聊的哈哦首付款是的老款繁花似锦符号 我打死福建师范部分科技水电费可接受的暴风科技舍不得看风景必部分科技水电费可接受的暴风科技舍不得看风景必</p>
      <p class="want">where</p>
      <p class="want-text">撒空间打不开居委会打卡机上班的会计师大部分科技水电费可接受的暴风科技舍不得看风景必胜客的解放碑接口和水电费会计厚大司考交话费收快递费看部分科技水电费可接受的暴风科技舍不得看风景必部分科技水电费可接受的暴风科技舍不得看风景必</p>
      <h4>技巧</h4>

      <table>
        <tr class="table-header">
          <td>软件</td>
          <td>使用经历</td>
          <td>熟练程度</td>
          <td>理解</td>
        </tr>
        <tr>
          <td>photoshop</td>
          <td>1</td>
          <td>1</td>
          <td>1</td>
        </tr>
        <tr class="bg-a">
          <td>1</td>
          <td>1</td>
          <td>1</td>
          <td>1</td>
        </tr>
        <tr>
          <td>1</td>
          <td>1</td>
          <td>1</td>
          <td>1</td>
        </tr>
        <tr class="bg-a">
          <td>1</td>
          <td>1</td>
          <td>1</td>
          <td>1</td>
        </tr>
      </table>
      <h4>经历</h4>
      <table>
        <tr class="table-header">
          <td>公司</td>
          <td>职位</td>
          <td>作品</td>
          <td>业绩</td>
        </tr>
        <tr>
          <td>1</td>
          <td>1</td>
          <td>1</td>
          <td>1</td>
        </tr>
        <tr class="bg-a">
          <td>1</td>
          <td>1</td>
          <td>1</td>
          <td>1</td>
        </tr>
      </table>
    </footer>
  </div>
</template>

<script>

export default {
  name: 'welcomeMan',
  data () {
    return {

    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style  scoped lang="scss">
@media screen and (max-width:940px){
  .welcomeMan{
    width:100%;
    height:100%;
    header{
      .header-top{
        height:50px;
        width:100%;
        background: #3f51b5;
      }
    }
  }
}

@media screen and (min-width:950px){
  .welcomeMan{
    width:100%;
    height:100%;
    header{
      .header-top{
        height:40px;
        width:100%;
        background: #3f51b5;
      }
      // .header-middle{
      //   height:50px;
      //   width:100%;
      //   background: #fff;
      // }
      .header-bottom{
        height:300px;
        width:100%;
        background: #252525;
        .middle{
          margin: 0 auto;
          width:900px;
          position: relative;
          height:100%;
          padding-top: 200px;
          color:#fff;
          h2{
            padding-left: 200px;
            letter-spacing: 2px;
          }
          p{
            padding-left: 216px;
            letter-spacing: 1px;
            color: #eee;
          }
          .myself{
            width:180px;
            height:180px;
            background: #777;
            position: absolute;
            top:200px;
          }
        }
      }
    }
    footer{
      width:900px;
      margin: 0 auto;
      padding-bottom: 100px;
      h4{
        padding-top: 50px;
      }
      .what{
        padding-left: 200px;
        padding-top: 20px;
        font-weight: bold;
        font-size: 18px;
      }
      .what-text{
        padding-left: 200px;
        color:#636363;
        width:800px;
      }
      .want{
        padding-left: 200px;
        font-weight: bold;
        font-size: 18px;
      }
      .want-text{
        color:#636363;
        padding-left: 200px;
        width:800px;
      }
    }
    table{
      box-shadow: 0 3px 6px rgba(0,0,0,.1);
      font-weight: bold;
    }
    tr{
      height:40px;
    }
    .table-header{
      background: #3f51b5;
      color:#fff;
    }
    td{
      width:200px;
      padding-left: 8px;
    }
    .bg-a{
      background: #f5f5f5;
    }
  }
}

</style>
