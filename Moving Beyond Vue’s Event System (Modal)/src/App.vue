<template>
  <div id="app">
    <div class="mt-2 ml-2">
      <button type="button" class="btn btn-primary" @click="open = true">
        Open
      </button>
    </div>

    <app-modal :show="open" @hide="open = false" />
  </div>
</template>

<script>
import AppModal from '@/components/Modal.vue';
import AppModal2 from '@/components/ModalWay2.vue';

export default {
  name: 'App',
  components: {
    AppModal,
    AppModal2
  },
  data() {
    return {
      open: false,
    };
  },

};
</script>

<style src="bootstrap/dist/css/bootstrap.css">
</style>
