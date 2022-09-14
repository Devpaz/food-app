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
  </div>
</template>
<style lang="less">
  .home {
    margin: 20px;
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
