<template>
    <MD />
</template>

<script>
import { defineComponent } from 'vue'
import { computed } from 'vue';
import { ref } from 'vue'
import { useRoute } from 'vue-router'

import MD from 'src/markdown/mdtest.md'

export default defineComponent({
  name: 'TestMD',
  components: {
    MD,
  },
  setup () {
    const route = useRoute()
    const source = ref(null)
    return {
      source,
    }
  },
  async beforeMount() {
    console.log('Source: ', this.source)
  },
})
</script>

