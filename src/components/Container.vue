<template>
    <div class="informer-container">
        <Temperature/>
        <div class="flex-break"></div>
        <Humidity/>
        <div class="vertical-divider"></div>
        <Wind/>
    </div>
</template>
<script>
import Temperature from './Temperature.vue'
import Humidity from './Humidity.vue'
import Wind from './Wind.vue'
export default {
    name: "Container",
    components:{
        Temperature,
        Humidity,
        Wind
    }
}
</script>

<style>
.informer-container {
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
  flex-wrap: wrap;
  width: 400px;
  padding: 30px;
  background-image: url('/img/forest.png');
  background-size: cover;
  background-position: center center;
  border-radius: 20px;
  box-shadow: 0px 0px 10px 0px rgba(50, 50, 50, 0.75);
}
.flex-break{
  flex-basis: 100%;
  height: 0;
}

.vertical-divider{
  height: 70px;
  width: 1px;
  background-color: #fff;
  vertical-align: middle;
  display: table-cell;
}
</style>