<template>
  <div class="talk">
    <header>
      <p>邓婧雯的个人作品集</p>
    </header>
    <main>

    </main>
    <footer>
      <div class="meeting" v-for="(nav,index) in talks" :key="nav.title">
        <router-link :to="{ name: 'talking', params: { id: nav.id }}">
          <div class="meeting-img">

          </div>
          <div class="meeting-title">
            <p>{{nav.title}}</p>
          </div>
          <div class="meeting-date">
            <p>{{nav.date}}</p>
          </div>
          <div class="meeting-where">
            <p>{{nav.where}}</p>
          </div>
          <div class="meeting-button">
            <button type="button" name="button">查看作品</button>
          </div>
        </router-link>
      </div>
    </footer>

    <div class="end">

    </div>

  </div>
</template>

<script>
import {talks} from '@/data'

export default {
  name: 'talk',
  data () {
    return {
      talks:talks
    }
  }
}
</script>

<style scoped lang="scss">
@media screen and (max-width:940px){
  .talk{
    height:100%;
    width:100%;
    position: relative;
    header{
      height:50px;
      width:100%;
      background: #3f51b5;
      position: fixed;
      top:0;
      left:0;
      z-index: 50;
      p{
        text-align: center;
        font-size: 15px;
        line-height: 50px;
        color:#fff;
      }
    }
    footer{
      padding: 15px;
      padding-top: 70px;
      height:100%;
      width:100%;
      background: #f5f5f5;
      .meeting{
        width:100%;
        background: #fff;
        box-shadow: 0 2px 6px rgba(0,0,0,.12);
        height:120px;
        margin-bottom: 15px;
        position: relative;

        p{
          margin: 0;
        }
        .meeting-img{
          width:120px;
          height:120px;
          background: #3f51b5;
          display: inline-block;
          float: left;
        }
        .meeting-title{
          font-size: 17px;
          padding: 10px 0 0 128px;
          font-weight: bold;
          color: #000;
        }
        .meeting-date{
          font-size: 13px;
          padding: 4px 0 0 128px;
          color:#777;
        }
        .meeting-where{
          font-size: 13px;
          padding: 2px 0 5px 128px;
          color:#777;
        }
        .meeting-button{
          width:80px;
          display: inline-block;
          font-size: 13px;
          color:#fff;
          background: #3f51b5;
          text-align: center;
          position: absolute;
          right:10px;
          bottom: 10px;
        }
      }
    }
  }
}
@media screen and (min-width:940px){
  .talk{
    height:100%;
    width:100%;
    position: relative;
    header{
      height:50px;
      width:100%;
      background: #3f51b5;
      position: fixed;
      top:0;
      left:0;
      z-index: 50;
      p{
        text-align: center;
        font-size: 18px;
        line-height: 50px;
        letter-spacing: 3px;
        color:#fff;
      }
    }
    main{
      height:500px;
      background: #777;
    }
    footer{
      padding: 15px;
      padding-top: 90px;
      width:100%;
      width:1200px;
      margin: 0 auto;
      .meeting{
        width:200px;
        background: #fff;
        box-shadow: 0 2px 6px rgba(0,0,0,.12);
        margin-bottom: 15px;
        position: relative;
        padding-bottom: 40px;
        display: inline-block;
        margin-left: 20px;
        border-radius: 3px;
        overflow: hidden;
        button{
          background: #3f51b5;
          border: 0;
        }
        p{
          margin: 0;
        }
        .meeting-img{
          width:200px;
          height:200px;
          background: #3f51b5;
          display: inline-block;
        }
        .meeting-title{
          font-size: 17px;
          padding: 10px 0 0 15px;
          font-weight: bold;
          color: #000;
        }
        .meeting-date{
          font-size: 13px;
          padding: 4px 0 0 15px;
          color:#777;
        }
        .meeting-where{
          font-size: 13px;
          padding: 2px 0 5px 15px;
          color:#777;
        }
        .meeting-button{
          width:80px;
          display: inline-block;
          font-size: 13px;
          color:#fff;
          background: #3f51b5;
          text-align: center;
          position: absolute;
          right:15px;
          bottom: 15px;
        }
      }
    }
    .end{
      background: #293646;
      height:250px;
      width:100%;
    }
  }
}


</style>
