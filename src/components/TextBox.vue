<template>
  <input type="text" class="input h30" v-model="val" placeholder>
</template>

<script>
export default {
  name: "TextBox",
  props: {
    val:String,
    msg: String
  }
};
</script>
