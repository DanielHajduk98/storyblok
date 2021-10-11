<template>
  <div
    v-editable="blok"
    class="py-8 mb-6 text-5xl font-bold text-center">
    <img class="h-48 w-full mb-4 object-cover" :src="blok.image.filename" :alt="blok.image.alt"/>
    {{ blok.headline }}
  </div>
</template>

<script>
export default {
  props: {
    blok: {
      type: Object,
      required: true
    }
  }
}
</script>
