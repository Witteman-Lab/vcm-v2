<template>
  <div>
    <div class="labels">
      <button class="languageBtn"
             @click="$emit('langswitch')"
      >{{ labels.currentLangue }}</button>
    </div>
  </div>
</template>
<script>
import config from "../assets/json/config.json"

export default {
  name: 'Navigation',
  components: {
  },

  data() {
    return {
      config
    }
  },
  props: ['labels'],

}
</script>
<style lang="scss">

.labels {
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
  align-items: center;

}
.languageBtn {
  border: solid;
  border-radius: 35px 35px 35px 35px;
  transition: 0.3s;
  background-color: #008363;
  color: #eeeeee;
}
</style>
