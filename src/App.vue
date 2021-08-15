<template>
  <q-dialog persistent :model-value="true">
    <div class="row">
      <div class="col-12">
        <q-input label="With v-model(Not-Updatable)" v-model="inputValue" />
      </div>
      <div class="col-12">
        <q-input label="Without v-model(Updatable)"></q-input>
      </div>
    </div>
  </q-dialog>
</template>

<script lang="ts">
import { defineComponent, ref } from "vue";

export default defineComponent({
  name: "App",
  components: {},
  setup() {
    const inputValue = ref("");
    return {
      inputValue,
    };
  },
});
</script>
