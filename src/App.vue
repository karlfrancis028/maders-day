<template>
  <div class="landing">
    <div class="landing__header">
      <img :src="$options.MothersDayVector" />
      <img :src="$options.Gif" />
    </div>
    <div class="landing__content">
      <img :src="$options.Image" />
      <div class="landing__message">
        <h1>Happy Mother's Day!!!</h1>
        <p>
          Hi, ma. Happy Mother's day! Thank you sa lahat ng sakripisyo mo sa amin hehehe. Hindi lang sa aming dalawa ni aya pati na din sa kamag-anak natin
          na binibigyan mo din. Alam ko na lahat ng pagsermon mo ay may dahilan at alam ko na ginagawa mo lang ito para din sa amin. Dahil doon, maraming salamat, mammeh. Labyu kahit mainitin ulo mo HEHEHE mwa. Happy mother's day! 
        </p>
      </div>
      <p class="landing__salutations">
        - Tet
        <br/>
        P.S. Kami ni Aya yung gumagalaw sa itaas 
      </p>
    </div>
  </div>
</template>

<script>
  import Image from '@/assets/mama.jpg';
  import MothersDayVector from '@/assets/mothers-day-vector.jpg';
  import Gif from '@/assets/tonton.gif';

  export default {
    name: 'App',
    Image,
    MothersDayVector,
    Gif,
  }
</script>

<style lang="scss">
  @import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&family=Rubik+Distressed&display=swap');

  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: "Poppins", sans-serif;
  }

  .landing {
    min-height: 100vh;

    &__header {
      display: flex;
      justify-content: center;
      margin-bottom: 16px;

      img {
        width: 180px;
        height: auto;
      }
    }

    &__content {
      img {
        width: 100%;
      }
    }

    &__message {
      padding: 10px;

      h1 {
        font-family: "Rubik Distressed", system-ui;
        font-weight: 400;
        color: rgb(250, 78, 78);
        font-style: normal;
        text-align: center;
        margin-bottom: 12px;
      } 
      
      p {
        font-size: 15px;
        font-weight: 300;
        text-align: justify;
        text-indent: 36px;
      }
    }

    &__salutations {
      padding: 10px;
      text-align: right;
      font-weight: 400;
    }
  }
</style>
