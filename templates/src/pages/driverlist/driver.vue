<template>
  <q-page class="flex flex-top">
<template>
  <div class="q-pa-md">
    <div class="q-gutter-y-md" style="max-width: 100%">
      <q-tabs
        v-model="detaillink"
      >
        <transition appear enter-active-class="animated zoomIn">
          <q-route-tab name="driverlist" :label="$t('driver.driver')" icon="img:statics/staff/driver.png" to="/driver/driverlist" exact/>
        </transition>
      </q-tabs>
    </div>
  </div>
</template>
    <router-view />
  </q-page>
</template>

<script>
export default {
  name: 'Pagedriver',
  data () {
    return {
      detaillink: 'driverlist'
    }
  },
  methods: {
  }
}
</script>
