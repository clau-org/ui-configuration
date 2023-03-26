<template>
  <div class="bg-red-500 h-screen">Hola</div>
</template>

<script setup>
  logger.info(
    'hola',
    prettyJson({
      hello: 'some json',
    }),
  )
</script>
