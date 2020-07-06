<template>
  <div>
    <p>myNewComponent Component</p>
    <sc-text :field="fields.heading" />
  </div>
</template>

<script>
import { Text } from '@sitecore-jss/sitecore-jss-vue';

export default {
  name: 'myNewComponent',
  components: {
    ScText: Text,
  },
  props: {
    fields: {
      type: Object,
      default: () => ({}),
    },
  },
}
</script>
