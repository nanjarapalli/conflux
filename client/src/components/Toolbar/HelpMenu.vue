<template>
   <q-btn color="grey-9" flat round icon="help">
      <q-menu>
         <div class="row no-wrap q-pa-md">
            <div class="column q-gutter-sm">
               <div class="text-overline">Help</div>
               <q-btn align="left" flat color="grey-9" label="Online Help" no-caps />
               <q-btn align="left" flat color="grey-9" label="What's New" no-caps />
               <q-btn align="left" flat color="grey-9" label="About Conflux" no-caps />

               <q-separator />

               <div class="text-overline">Legal</div>
               <q-btn align="left" flat color="grey-9" label="Terms of Service" no-caps />
               <q-btn align="left" flat color="grey-9" label="Privacy Policy" no-caps />

               <q-separator />

               <div class="q-mt-md text-caption text-italic text-grey-7 row justify-center">Conflux v{{version}}</div>
            </div>
         </div>
      </q-menu>
   </q-btn>
</template>

<script>
import { mapState } from 'vuex'

export default {
   computed: {
      ...mapState('app', ['version'])
   }

}
</script>

<style scoped>

</style>
