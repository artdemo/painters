<template>
  <div class='card'>
    <img :src="card.imageUrl" alt="" class='card__img'/>
  </div>
</template>

<script>
export default {
  name: 'Card',
  props: ['card'],
};
</script>

<style lang='scss' scoped>
// @import "../../scss/_global.scss";
// @import "../scss/_global.scss";
// @import "./scss/_global.scss";

.card {
    border: 2px dashed orange;
    width: 33.33%;

    &__img {
        width: 100%;
        display: block;
    }

}
</style>
