<template>
  <div class="q-pa-md q-gutter-md">
    <div>
      <q-btn-toggle
        v-model="modelA"
        multiple
        push
        glossy
        toggle-color="primary"
        :options="[
          { label: '1', value: 1 },
          { label: '2', value: 2 },
          { label: '3', value: 3 },
          { label: '4', value: 4 },
          { label: '5', value: 5 },
          { label: '6', value: 6 },
          { label: '7', value: 7 },
          { label: '8', value: 8 },
          { label: '9', value: 9 },
          { label: '10', value: 10 },
        ]"
      />
    </div>
    <div>
      <q-btn-toggle
        v-model="modelB"
        multiple
        push
        glossy
        toggle-color="primary"
        :options="[
          { label: 'Bold', value: 'bold' },
          { label: 'Italic', value: 'italic' },
          { label: 'Underline', value: 'underline' },
          { label: 'Subscript', value: 'subscript' },
        ]"
      />
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      modelA: [ 5, 9 ],
      modelB: [ 'bold', 'italic' ]
    }
  }
}
</script>
