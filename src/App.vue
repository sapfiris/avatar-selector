<template>
  <div id="app">
    <AvatarSelector v-model="file" :formats="formats" :size="sizeKB" />
  </div>
</template>

<script>
import AvatarSelector from './components/AvatarSelector';

export default {
  name: 'App',
  data() {
    return {
      file: null,
      formats: ['image/jpg', 'image/jpeg', 'image/png'],
      sizeKB: 700
    };
  },
  components: {
    AvatarSelector
  }
}
</script>
