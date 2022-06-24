<template>
  <div class="baseContainer">
    <h4>Онлайн-помощница по обращению в полицию</h4>
    <span class="text">
    <p>Мы поможем вам заполнить обращение в МВД, а также расскажем, как зафиксировать физическое насилие и где найти
      ближайшие шелтеры для укрытия.
    </p>
    <p>Сайт предназначен для тех, у кого нет адвоката или возможности его пригласить.
    </p>
      </span>
    <span class="textGrey">
    <q-icon name="fas fa-exclamation-circle"/>
     Если вы живете в регионах, где работают правозащитные организации, обязательно свяжитесь с ними.
  </span>
    <div class="q-pa-md q-gutter-sm">
      <q-btn to="/" color="white" text-color="black" label="Заполнить обращение в полицию"/>
      <q-btn color="white" text-color="black" label="Как зафиксировать физ.насилие"/>
      <q-btn to="/shelter" color="white" text-color="black" label="Где можно укрыться"/>
    </div>


  </div>
</template>

<script>
  import {defineComponent} from 'vue'

  export default defineComponent({
    name: 'HomePage'
  })
</script>

<style lang="css">
  .baseContainer {
    font-family: 'Montserrat';
    margin-left: 3vw;
  }

  .text {
    font-size: 18px;
  }

  .textGrey {
    display: inline-flex;
    background-color: #E8E8E8;
    border-radius: 5px;
    align-items: center;
    font-style: normal;
    font-size: 18px;
    /*or 25px*/
  }

  .textGrey i {
    margin-right: 5px;
  }


</style>


