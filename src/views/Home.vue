<template>
  <div class="home">
    <div class="header">
      <h2 class="title">Hi <b>Paolo !</b></h2>
      <div class="input">
        <input type="text" placeholder="Find what you want">
        <div class="icon-input">
          <i class='bx bx-search'></i>
        </div>
      </div>
      <div class="combo-header">
        <div class="text">
          <h3>Free Combo</h3>
          <p>Burger + Coca-cola for new users</p>
        </div>
        <div class="img">
          <img src="https://images.unsplash.com/photo-1586190848861-99aa4a171e90?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=880&q=80" alt="">
        </div>
      </div>
    </div> 
    <div class="scroll-menu">
      <div class="scroll-content">
        <div :key="index" class="avatar" v-for="(item,index) in 10">
          <i class='bx bx-beer bx-sm'></i> 
        </div>
      </div>
    </div>
    <h2>Top Products</h2>
    <div class="scroll-menu">
      <div class="scroll-content">
        <div :key="index" v-for="(item, index) in 10" class="top-products">
          <div class="top-products-img">
            <img src="https://images.unsplash.com/photo-1607547023949-e07be8732b3e?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MTl8fGp1aWNlJTIwb3JhbmNlfGVufDB8fDB8fA%3D%3D&auto=format&fit=crop&w=700&q=60" alt="">
          </div>


          <div class="top-products-text">
            <div class="top-products-title">Berry Juice</div>
            <div class="top-products-price">$ 7.5</div>
          </div>
          <i class='bx bx-plus-medical'></i>

        </div>
      </div>
    </div>
  </div>
</template>
<style lang="less">
  h2 {
    margin-top: 15px;
    font-weight: 400;

  }
  .home {
    margin: 20px;
    .top-products {
      position: relative;
      min-width: 150px;
      background-color: rgba(250, 248, 248);
      padding: 10px;
      border-radius: 10px;
      .card-footer {
        display: flex;
      }
      i {
        position: absolute;
        right: 0;
        bottom: 0;
        padding: 10px;
        color: white;
        border-radius: 50px;
        background-color: rgba(74, 174, 84);
        margin: 5px;
      }
      .top-products-img {
        img {
          width: 100%;
        }
      }
      .top-products-text {
        .top-products-title {
          color: rgba(47, 47, 47)
        }
        .top-products-price {
          color: rgba(255, 131, 62);
        }
      }
    }
    .scroll-menu {
      margin-top: 10px ;
      .scroll-content {
        display: flex;
        overflow-y: auto;
        .avatar {
          background-color: rgb(250, 248, 248) ;
          padding: 20px;
          border-radius: 10px;
          margin: 10px;
          i {
            color: rgba(255, 131, 62);
          }
        }
      }
    }
  }
  .title {
    font-weight: 350;
  }
  .header {
    .combo-header {
      background-color: rgba(74, 174, 84);
      color: white;
      padding: 10px;
      border-radius: 20px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-top: 20px;
      .img {
        width: 50%;
        img{
          width: 100%;
          object-fit: cover;
        }
        width: 50%;
        object-fit: cover;
      }
      .text {
        width: 50%;
        h3 {
          font-weight: 600;
        }
        p {
          font-weight: 300;
        }
      }
    }
    .input {
      display: flex;
      position: relative;
      align-items: center;
      margin-top: 15px;
      input {
        width: 100%;
        background-color: rgba(250, 248, 248);
        border: 0px;
        outline: none;
        padding: 10px;
        padding-left: 30px;
        border-radius: 10px;
      }
      .icon-input {
        position: absolute;
        margin-left: 10px;
      }
    }
    .title {
      font-weight: 350;
    }
  }
</style>
