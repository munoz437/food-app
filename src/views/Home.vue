<template>
  <div class="home">
    <div class="header">
      <div class="img-logo">
        <img
          src="https://donaluisaxicotencatl.com/wp-content/uploads/2020/09/cropped-Dona-Luisa-Xicotencatl-Antigua-Guatemala-1.png"
          alt=""
        />
      </div>

      <h2 class="title">
        <b>DOÑA LUISA XICOTENCATL</b>
      </h2>

      <div class="input">
        <input type="text" placeholder="Buscar..." />
        <div class="icon-input">
          <i class="bx bx-search"></i>
        </div>
      </div>

      <div class="combo-header">
        <div class="text">
          <b><h3>QUESO BURGUESA</h3></b>
          <p>
            Torta de carne asada, cubierta con queso cheddar derretido, con pan
            integral.
          </p>
        </div>
        <!--cambiar la imagen-->
        <div class="img">
          <img
            src="https://donaluisaxicotencatl.com/wp-content/uploads/2020/09/Hamburguesa-de-Dona-Luisa-Xicotencatl-1024x643.jpg"
            alt=""
          />
        </div>
      </div>
    </div>
    <div class="scroll-menu">
      <!--modificar-->
      <div class="scroll-content">
        <!--<div :key="index" class="avatar" v-for="(item, index) in 10">-->
        <div class="avatar">
          <i class="bx bxs-drink bx-sm"></i>
        </div>
        <div class="avatar">
          <i class="bx bxs-coffee bx-sm"></i>
        </div>

        <div class="avatar">
          <i class="bx bx-dish bx-sm"></i>
        </div>

        <div class="avatar">
          <i class="bx bx-cake bx-sm"></i>
        </div>
      </div>
    </div>

    <!--BEBIDAS FRÍAS-->
    <h2>Bebidas Frías</h2>
    <div class="scroll-menu">
      <!--modificar-->
      <div class="scroll-content">
        <!--<div :key="index" v-for="(item, index) in 10" class="top-products">-->
        <div :key="frias" v-for="frias in bFrias" class="top-products">
          <div class="top-products-img">
            <img
              src="http://donaluisaxicotencatl.com/wp-content/uploads/2020/09/Menu-Dona-Luisa-Xicotencatl-2-1024x680.jpg"
              alt=""
            />
          </div>

          <div class="top-products-text">
            <b><div class="top-products-title">{{ frias.titulo}}</div> </b>
            <div class="top-products-title">{{ frias.descripcion }}</div>
            <div class="top-products-price">Q {{ frias.precio }}.00</div>
          </div>

          <i class="bx bx-plus-medical"></i>
        </div>
      </div>
    </div>

    <!--BEBIDAS CALIENTES-->
    <h2>Bebidas Calientes</h2>
    <div class="scroll-menu">
      <!--modificar-->
      <div class="scroll-content">
        <div
          :key="bCaliente"
          v-for="bCaliente in bCalientes"
          class="top-products"
        >
          <div class="top-products-img">
            <img
              src="https://donaluisaxicotencatl.com/wp-content/uploads/2020/09/Dona-Luisa-Xicotencatl-Cafe-1024x736.jpg"
              alt=""
            />
          </div>

          <div class="top-products-text">
            <b><div class="top-products-title">{{ bCaliente.titulo}}</div> </b>
            <div class="top-products-title">{{ bCaliente.descripcion }}</div>
            <div class="top-products-price">Q.{{ bCaliente.precio }}.00</div>
          </div>

          <i class="bx bx-plus-medical"></i>
        </div>
      </div>
    </div>

    <!--DESAYUNOS-->
    <h2>Desayunos</h2>
    <div class="scroll-menu">
      <!--modificar-->
      <div class="scroll-content">
        <div :key="desayuno" v-for="desayuno in desayunos" class="top-products">
          <div class="top-products-img">
            <img
              src="https://donaluisaxicotencatl.com/wp-content/uploads/2020/09/Dona-Luisa-Xicotencatl-Cafe-1024x736.jpg"
              alt=""
            />
          </div>

          <div class="top-products-text">
            <b
              ><div class="top-products-title">{{ desayuno.titulo }}</div></b
            >
            <div class="top-products-title">{{ desayuno.descripcion }}</div>
            <div class="top-products-price">Q{{ desayuno.precio }}.00</div>
          </div>

          <i class="bx bx-plus-medical"></i>
        </div>
      </div>
    </div>

    <!--SOPAS-->
    <h2>Sopas</h2>
    <div class="scroll-menu">
      <!--modificar-->
      <div class="scroll-content">
        <div :key="sopa" v-for="sopa in sopas" class="top-products">
          <div class="top-products-img">
            <img
              src="https://donaluisaxicotencatl.com/wp-content/uploads/2020/09/Dona-Luisa-Xicotencatl-Cafe-1024x736.jpg"
              alt=""
            />
          </div>

          <div class="top-products-text">
            <b
              ><div class="top-products-title">{{ sopa.titulo }}</div></b
            >
            <div class="top-products-title">{{ sopa.descripcion }}</div>
            <div class="top-products-price">Q{{ sopa.precio }}.00</div>
          </div>

          <i class="bx bx-plus-medical"></i>
        </div>
      </div>
    </div>

    <!--INFANTILES-->
    <h2>Infantiles</h2>
    <div class="scroll-menu">
      <!--modificar-->
      <div class="scroll-content">
        <div
          :key="infantil"
          v-for="infantil in infantiles"
          class="top-products"
        >
          <div class="top-products-img">
            <img
              src="https://donaluisaxicotencatl.com/wp-content/uploads/2020/09/Dona-Luisa-Xicotencatl-Cafe-1024x736.jpg"
              alt=""
            />
          </div>

          <div class="top-products-text">
            <b
              ><div class="top-products-title">{{ infantil.titulo }}</div></b
            >
            <div class="top-products-title">{{ infantil.descripcion }}</div>
            <div class="top-products-price">Q{{ infantil.precio }}.00</div>
          </div>

          <i class="bx bx-plus-medical"></i>
        </div>
      </div>
    </div>

    <!--SANDWICHES-->
    <h2>Sandwiches</h2>
    <div class="scroll-menu">
      <!--modificar-->
      <div class="scroll-content">
        <div
          :key="sandwich"
          v-for="sandwich in sandwiches"
          class="top-products"
        >
          <div class="top-products-img">
            <img
              src="https://donaluisaxicotencatl.com/wp-content/uploads/2020/09/Dona-Luisa-Xicotencatl-Cafe-1024x736.jpg"
              alt=""
            />
          </div>

          <div class="top-products-text">
            <b><div class="top-products-title">{{ sandwich.titulo }}</div></b>
            <div class="top-products-title">{{sandwich.descripcion}}</div>
            <div class="top-products-price">Q{{sandwich.precio}}.00</div>
          </div>

          <i class="bx bx-plus-medical"></i>
        </div>
      </div>
    </div>

    <!--HAMBURGUESAS-->
    <h2>Hamburguesas</h2>
    <div class="scroll-menu">
      <!--modificar-->
      <div class="scroll-content">
        <div
          :key="hamburguesa"
          v-for="hamburguesa in hamburguesas"
          class="top-products"
        >
          <div class="top-products-img">
            <img
              src="https://donaluisaxicotencatl.com/wp-content/uploads/2020/09/Dona-Luisa-Xicotencatl-Cafe-1024x736.jpg"
              alt=""
            />
          </div>

          <div class="top-products-text">
            <b>
              <div class="top-products-title">{{ hamburguesa.titulo }}</div>
            </b>
            <div class="top-products-title">{{ hamburguesa.descripcion }}</div>
            <div class="top-products-price">Q{{ hamburguesa.precio }}.00</div>
          </div>

          <i class="bx bx-plus-medical"></i>
        </div>
      </div>
    </div>

    <!--PAPAS RELLENAS-->
    <h2>Papas Rellenas</h2>
    <div class="scroll-menu">
      <!--modificar-->
      <div class="scroll-content">
        <div :key="papas_rellena" v-for="papas_rellena in papas_rellenas" class="top-products">
          <div class="top-products-img">
            <img
              src="https://donaluisaxicotencatl.com/wp-content/uploads/2020/09/Dona-Luisa-Xicotencatl-Cafe-1024x736.jpg"
              alt=""
            />
          </div>

          <div class="top-products-text">
            <b>
            <div class="top-products-title">{{ papas_rellena.titulo }}</div></b>
            <div class="top-products-title">{{ papas_rellena.descripcion }}</div>
            <div class="top-products-price">Q{{ papas_rellena.precio }}.00</div>
          </div>

          <i class="bx bx-plus-medical"></i>
        </div>
      </div>
    </div>

    <!--POSTRES-->
    <h2>Postres</h2>
    <div class="scroll-menu">
      <!--modificar-->
      <div class="scroll-content">
        <div :key="postre" v-for="postre in postres" class="top-products">
          <div class="top-products-img">
            <img
              src="https://donaluisaxicotencatl.com/wp-content/uploads/2020/09/Dona-Luisa-Xicotencatl-Cafe-1024x736.jpg"
              alt=""
            />
          </div>

          <div class="top-products-text">
            <b><div class="top-products-title">{{ postre.titulo }}</div></b>
            <div class="top-products-title">{{ postre.descripcion }}</div>
            <div class="top-products-price">Q{{ postre.precio }}.00</div>
          </div>

          <i class="bx bx-plus-medical"></i>
        </div>
      </div>
    </div>

    <!--HELADOS-->
    <h2>Helados</h2>
    <div class="scroll-menu">
      <!--modificar-->
      <div class="scroll-content">
        <div :key="helado" v-for="helado in helados" class="top-products">
          <div class="top-products-img">
            <img
              src="https://donaluisaxicotencatl.com/wp-content/uploads/2020/09/Dona-Luisa-Xicotencatl-Cafe-1024x736.jpg"
              alt=""
            />
          </div>

          <div class="top-products-text">
            <b><div class="top-products-title">{{ helado.titulo}}</div> </b>
            <div class="top-products-title">{{ helado.descripcion}}</div>
            <div class="top-products-price">Q{{ helado.precio}}.00</div>
          </div>

          <i class="bx bx-plus-medical"></i>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
//CODIGO PARA LOS PRODUCTOS
export default {
  name: "tarea",
  data() {
    return {
      bFrias: [
        {
          titulo: "Jugo de Naranja Natural Pequeño 9 Onz.",
          precio: 13,
          descripcion: "Servido fresco cada mañana.",
        },
        {
          titulo: " Jugo de Naranja Natural Grande 12 Onz. ",
          precio: 17,
          descripcion: "Servido fresco cada mañana.",
        },
        {
          titulo: "Limonada o Naranjada",
          precio: 15,
          descripcion: "Con soda o con agua.",
        },
        {
          titulo: "Licuado con Leche 16 Onz.",
          precio: 17,
          descripcion:
            "Rico y espeso con su selección de frutas naturales, banano, melón, papaya, piña o sandía.",
        },
        {
          titulo: "Licuado con Agua 16 Onz.",
          precio: 13,
          descripcion:
            "Con su selección de frutas naturales, banano, melón, papaya, piña o sandía.",
        },
        {
          titulo: "Licuado con Yogurt 16 Onz.",
          precio: 22,
          descripcion:
            "preparado con el yogurt hecho en casa, con frutas naturales, banano, melón, papaya, piña o sandía.",
        },
        {
          titulo: "Aguas Gaseosas",
          precio: 12,
          descripcion:
            "una selección de sabores populares.(Aguas Gaseosas Dietéticas Q12)",
        },
        {
          titulo: " Agua Pura Botella 16 Onz.",
          precio: 4,
          descripcion: "",
        },
        {
          titulo: "Refrescos 16 Onz.",
          precio: 12,
          descripcion: "natural y tradicional de Horchata o Jamaica.",
        },
        {
          titulo: " Milk Shake ",
          precio: 30,
          descripcion:
            "Escoja su sabor favorito de nuestros helados, vainilla, fresa, chocolate, galleta, pistacho.",
        },
        {
          titulo: "Cafe Glacé ",
          precio: 30,
          descripcion:
            "la mejor combinación de helado y café expresso, batido, con canela encima.",
        },

        {
          titulo: "Cerveza Gallo",
          precio: 18,
          descripcion: "Servida bien fría.",
        },
      ],
      bCalientes: [
        {
          titulo: "Café Negro",
          precio: 9,
          descripcion: "el mejor café de Guatemala con su segunda taza gratis.",
        },
        {
          titulo: "Café con Leche",
          precio: 11,
          descripcion: "",
        },
        {
          titulo: "Café Sanka",
          precio: 8,
          descripcion: "",
        },
        {
          titulo: "Café Expresso",
          precio: 7,
          descripcion: "estilo italiano, bien fuerte y aromático.",
        },
        {
          titulo: "Café Capuchino",
          precio: 12,
          descripcion:
            "una combinacion de expresso y leche espumada por vapor.",
        },
        {
          titulo: "Té",
          precio: 7,
          descripcion: "una selección de sabores naturales.",
        },
        {
          titulo: "Chocolate Caliente",
          precio: 12,
          descripcion: "preparado con Agua o Leche.",
        },
      ],
      desayunos: [
        {
          titulo: "Fruta Mixta",
          precio: 25,
          descripcion: "una porción abundante de frutas frescas.",
        },
        {
          titulo: "Yogurt",
          precio: 16,
          descripcion: " hecho diariamente en casa con ingredientes naturales.",
        },
        {
          titulo: "Huevos de la Casa",
          precio: 22,
          descripcion:
            "2 huevos al gusto (estrellados, revueltos, tibios o poche) con frijoles, panecillos tostados, mantequilla y jalea.",
        },
        {
          titulo: "Huevos Rancheros",
          precio: 23,
          descripcion:
            "2 huevos estrellados con una salsa fresca de tomate con frijoles y panecillos tostados.",
        },
        {
          titulo: "Huevos al Oeste",
          precio: 26,
          descripcion:
            "2 huevos revueltos con cebolla, tomate, chile pimiento y jamón picados, servido con frijoles y panecillos tostados.",
        },
        {
          titulo: "Torre de Huevos",
          precio: 33,
          descripcion:
            "2 huevos, jamón y queso cheddar derretido sobre panecillos tostados.",
        },
        {
          titulo: "Omelet y Panecillo",
          precio: 35,
          descripcion:
            "un desayuno clásico con 3 huevos preparado con su selección de jamón y queso, verduras frescas, atún o champiñones.",
        },
        {
          titulo: "Granola con Banano",
          precio: 20,
          descripcion:
            "nuestra receta hecha en casa con leche y rodajas de banano encima.",
        },
        {
          titulo: "Granola con Fruta y Yogurt",
          precio: 47,
          descripcion:
            "el desayuno natural con una selección de fruta tropical, granola y nuestro fresco yogurt, todo hecho en casa.",
        },
        {
          titulo: "Granola con Fruta y Yogurt",
          precio: 47,
          descripcion:
            "el desayuno natural con una selección de fruta tropical, granola y nuestro fresco yogurt, todo hecho en casa.",
        },
        {
          titulo: "Corn Flakes con Banano",
          precio: 16,
          descripcion: "el desayuno tradicional servido con leche.",
        },
        {
          titulo: "Tostadas Francesas",
          precio: 22,
          descripcion:
            "hechas con pan integral o de pasas con canela, servidas con jarabe o miel.",
        },
        {
          titulo: "Panqueques Americanos",
          precio: 22,
          descripcion:
            "2 panqueques grandes de harina integral o harina blanca, servidos con jarabe o miel.",
        },
        {
          titulo: "Pan Tostado o Panecillo",
          precio: 12,
          descripcion: "servido con mantequilla, jalea o miel.",
        },
        {
          titulo: "Refacción del dia",
          precio: 12,
          descripcion:
            "de lunes a viernes de 9:00 a 11:00 am. Una selección de panitos ricos, calientes del horno, servidos con café gratis.",
        },
        {
          titulo: "Frijoles Parados",
          precio: 6,
          descripcion: "cocinados al estilo antigüeño.",
        },
        {
          titulo: "Tocino",
          precio: 14,
          descripcion: "una porción generosa, frito a su gusto.",
        },
      ],
      sopas: [
        {
          titulo: "Sopa Vegetariana",
          precio: 18,
          descripcion:
            "hecha diariamente con verduras frescas, servida con pan tostado.",
        },
        {
          titulo: "Chile con Carne",
          precio: 24,
          descripcion:
            "preparado con frijoles colorados, carne molida y una salsa medio picante de tomate, servido con pan tostado.",
        },
      ],
      infantiles: [
        {
          titulo: "Desayuno",
          precio: 26,
          descripcion:
            "jugo de Naranja pequeño, 2 Panqueques con carita alegre, servido con fruta a su elección.",
        },
        {
          titulo: "Almuerzo o cena",
          precio: 26,
          descripcion:
            "licuado de Fruta ½ Sándwich de Jamón y Queso, servido con papalinas, y uno de nuestros diferentes sabores de helado.",
        },
      ],
      sandwiches: [
        {
          titulo: "Roast Beef",
          precio: 0,
          descripcion:
            "rodajas de carne horneada con pan caliente a la plancha.",
        },
        {
          titulo: "Jamón y Queso Cheddar",
          precio: 0,
          descripcion: "con pan frito y dorado a su perfección.",
        },
        {
          titulo: "California Super",
          precio: 0,
          descripcion:
            "una combinación natural de aguacate, retoño y queso chedar.",
        },
        {
          titulo: "Ensalada de Pollo",
          precio: 0,
          descripcion:
            "pollo picado con verduras (chile pimiento, cebolla, apio, huevo duro y perejil) mezclado con mayonesa.",
        },
        {
          titulo: "Pollo Dietetico",
          precio: 0,
          descripcion:
            "pollo picado con verduras (chile pimiento, cebolla, apio, huevo duro y perejil) mezclado con yogurth.",
        },
        {
          titulo: "Atún",
          precio: 0,
          descripcion: "atún mezclado con cebolla picada y mayonesa.",
        },
        {
          titulo: "Atún dietetico",
          precio: 0,
          descripcion:
            "atun mezclado con cebolla picada y yogurth, acompañado con fruta.",
        },
        {
          titulo: "Tex-Mex Tostadas",
          precio: 0,
          descripcion:
            "capas de carne tejana (o frijoles para los vegetarianos) con lechuga, tomate, cebolla, queso y salsa encima de tortillas fritas.",
        },
        {
          titulo: "Mini Pizza",
          precio: 0,
          descripcion:
            "panecillos tostados con salsa italiana, salami y queso mozzarella.",
        },
        {
          titulo: "DLX Combo",
          precio: 44,
          descripcion:
            "Sopa del día con cualquier sándwich de los números 48 al 56) y una bebida.",
        },
        {
          titulo: "Club Sandwich",
          precio: 42,
          descripcion:
            "preparado con 3 rodajas de pan tostado, tocino, queso, pollo, lechuga, tomate.",
        },
        {
          titulo: "Sandwich de Pechuga de Pollo",
          precio: 35,
          descripcion: "pechuga horneada con especies y semilla de amapola.",
        },
      ],
      hamburguesas: [
        {
          titulo: "Burguer Simple",
          precio: 33,
          descripcion: "Torta de carne asada con pan integral.",
        },
        {
          titulo: "Burguer California",
          precio: 40,
          descripcion:
            "torta de carne asada, cubierta con aguacate y retoño de alfalfa, con pan integral.",
        },
        {
          titulo: "Queso Burguesa",
          precio: 37,
          descripcion:
            "torta de carne asada, cubierta con queso cheddar derretido, con pan integral.",
        },
        {
          titulo: "Tocino Burguesa",
          precio: 40,
          descripcion:
            "torta de carne asada con queso y tiras de tocino, con pan integral.",
        },
        {
          titulo: "Burguer Vegetariano",
          precio: 33,
          descripcion:
            "Una combinación de sabrosa de tofu y verduras picadas en una torta, con pan integral.",
        },
      ],
      papas_rellenas: [
        {
          titulo: "Papas Rellenas con Queso",
          precio: 28,
          descripcion:
            "papas horneadas con queso derretido simple o jalapeño acompañado con pan tostado.",
        },
        {
          titulo: "Papas y Chile con Carne",
          precio: 30,
          descripcion:
            "papas horneadas con queso derretido encima de una porción de chile con carne y pan tostado.",
        },
        {
          titulo: "Papas con Queso y Tocino",
          precio: 34,
          descripcion:
            "papas horneadas con queso derretido y tiras de tocino, con pan tostado.",
        },
        {
          titulo: "Papas fritas",
          precio: 9,
          descripcion: "las favoritas de todos.",
        },
      ],
      postres: [
        {
          titulo: "Pasteles y Pays",
          precio: 12,
          descripcion:
            "una variedad de sabores distintos cada día, hechos en casa.",
        },
        {
          titulo: "Pasteles Fríos",
          precio: 17,
          descripcion:
            "una variedad de sabores con crema batida, distintos cada día.",
        },
        {
          titulo: "Galletas",
          precio: 8,
          descripcion: "la galleta gigante de Antigua.",
        },
      ],
      helados: [
        {
          titulo: "Una Bola en Cono o Copa",
          precio: 14,
          descripcion: "",
        },
        {
          titulo: "Pastel Sundae",
          precio: 30,
          descripcion:
            "sobre pastel de chocolate 2 bolas de helado de vainilla y café, adornado con salsa de chocolate y caramelo con nueces de almendra picada.",
        },
      ],
    };
  },
};
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
      &::-webkit-scrollbar {
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
  .img-logo {
    img {
      display: block;
      margin-left: auto;
      margin-right: auto;
    }
  }
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
    margin-top: 20px;
    text-align: center;
  }
}
</style>
