<template>
    <Members />
</template>

<script>
  import { Component, Vue } from 'vue-property-decorator';
  import Members from '../components/Members.vue';

  @Component({
    components: {
      Members,
    },
  })
  export default class MemberList  extends Vue {}
</script>