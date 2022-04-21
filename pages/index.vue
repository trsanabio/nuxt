<template>

  <div>

    <pre>
      <!-- state por ser um módulo e user pelo nome do módulo na pasta store -->
      {{ $store.state.user }}
    </pre>

    <!-- <button v-tooltip="'You have ' + count + ' new messages.'"> -->

    <pre>
      <!-- user foi mapeado no computed deste arquivo -->
      {{ user }}
    </pre>

  </div>

  <!-- <Tutorial/> -->
</template>

<script>
import { mapState } from 'vuex';
export default {
  name: 'IndexPage',

  data (){
    return {

    }
  },

  mounted () {
    console.log(this.$name('Thyago Ramos Sanabio'));
    console.log(this.$dayjs().format());
  },

  computed: {
    ...mapState({
      user: state => state.user
    })
  },

}
</script>
