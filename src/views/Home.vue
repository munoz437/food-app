<template>
  <div class="home">
    <div class="header">
      <h2 class="title">Hi <b>!</b></h2>

      <div class="input">
        <input type="text" placeholder="Buscar..." />
        <div class="icon-input">
          <i class="bx bx-search"></i>
        </div>
      </div>

      <div class="combo-header">
        <div class="text">
          <h3>Combo de Oferta</h3>
          <p>descripcion...</p>
        </div>
        <!--cambiar la imagen-->
        <div class="img">
          <img
            src="https://images.unsplash.com/photo-1485451456034-3f9391c6f769?ixlib=rb-1.2.1&ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&auto=format&fit=crop&w=1050&q=80"
            alt=""
          />
        </div>
      </div>
    </div>
    <div class="scroll-menu">
      <!--modificar-->
      <div class="scroll-content">
        <div :key="index" class="avatar" v-for="(item, index) in 10">
          <i class="bx bxs-pizza bx-sm"></i>
        </div>
      </div>
    </div>

    <h2>Top Products</h2>
    <div class="scroll-menu">
      <!--modificar-->
      <div class="scroll-content">
        <div :key="index" v-for="(item, index) in 10" class="top-products">
          <div class="top-products-img">
            <img
              src="https://images.unsplash.com/photo-1594212699903-ec8a3eca50f5?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=1051&q=80"
              alt=""
            />
          </div>

          <div class="top-products-text">
            <div class="top-products-title">jugos</div>
            <div class="top-products-price">$7.5</div>
          </div>

          <i class="bx bx-plus-medical"></i>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
/*
AQUI VA EL JAVASCRIPT
*/
</script>

<style lang="less">
h2 {
  font-weight: 400;
}
.home {
 
  .scroll-menu-top {
    .scroll-content-top {
      display: flex;
    }
  }

  .top-products {
    background-color: rgba(250, 248, 248);
    padding: 10px;
    border-radius: 10px;
    .top-products-img {
      img {
        width: 100%;
        border-radius: 10px;
      }
    }
    position: relative;
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
    min-width: 150px;
    .top-products-text {
      margin-top: 10px;
      .top-products-price {
        color: rgba(255, 131, 62);
      }

      .top-products-title {
        color: rgba(47, 47, 47);
      }
    }
  }
  margin: 20px;

  .scroll-menu {
    margin-top: 10px;
    .scroll-content {
      display: flex;
      overflow-y: auto;
      &::-webkit-scrollbar{
        display: none;
      }
      .avatar {
        background-color: rgba(250, 248, 248);
        padding: 20px;
        border-radius: 10px;
        margin: 2px;
        i {
          color: rgba(255, 131, 62);
        }
      }
    }
  }
}
.header {
  .combo-header {
    background: rgba(74, 174, 84);
    color: white;
    padding: 20px;
    border-radius: 20px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-top: 20px;
    .img {
      width: 50%;
      img {
        width: 100%;
        object-fit: cover;
        border-radius: 10px;
      }
    }
    .text {
      width: 50%;
      h3 {
        font-weight: 400;
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
      background: rgba(250, 248, 248);
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
     margin-top: 60px;
  }
}
</style>
