<template>
  <div id="banners">
    <c-tabs orientation="vertical" variant="unstyled" @change="setActiveTab">
      <c-grid id="info" align-items="start" template-columns="20% 80%">
        <c-grid-item>
          <c-tab-list>
            <c-tab>
              <tab-switcher
                :active-image="pathForImage('ho_us1@3x.png')"
                :inactive-image="pathForImage('ho_us2@3x.png')"
                :index="0"
                :active-tab="activeTab"
            /></c-tab>

            <c-tab>
              <tab-switcher
                :active-image="pathForImage('ho_li1@3x.png')"
                :inactive-image="pathForImage('ho_li2@3x.png')"
                :index="1"
                :active-tab="activeTab"
            /></c-tab>

            <c-tab>
              <tab-switcher
                :active-image="pathForImage('ho_sp1@3x.png')"
                :inactive-image="pathForImage('ho_sp2@3x.png')"
                :index="2"
                :active-tab="activeTab"
            /></c-tab>

            <c-tab>
              <tab-switcher
                :active-image="pathForImage('ho_lo1@3x.png')"
                :inactive-image="pathForImage('ho_lo2@3x.png')"
                :index="3"
                :active-tab="activeTab"
            /></c-tab>

            <c-tab>
              <tab-switcher
                :active-image="pathForImage('ho_po1@3x.png')"
                :inactive-image="pathForImage('ho_po2@3x.png')"
                :index="4"
                :active-tab="activeTab"
            /></c-tab>

            <c-tab>
              <tab-switcher
                :active-image="pathForImage('ho_ga1@3x.png')"
                :inactive-image="pathForImage('ho_ga2@3x.png')"
                :index="5"
                :active-tab="activeTab"
            /></c-tab>
          </c-tab-list>
        </c-grid-item>

        <c-grid-item>
          <c-tab-panels>
            <c-tab-panel>
              <img
                v-chakra
                width="100%"
                pr="0.8em"
                border-radius="0.5em"
                mb="0.6em"
                src="~/assets/images/banner9.png"
              />
              <img
                v-chakra
                width="100%"
                pr="0.8em"
                border-radius="0.5em"
                mb="0.6em"
                src="~/assets/images/banner8.png"
              />
              <img
                v-chakra
                width="100%"
                pr="0.8em"
                border-radius="0.5em"
                mb="0.6em"
                src="~/assets/images/banner10.png"
              />
              <img
                v-chakra
                width="100%"
                pr="0.8em"
                border-radius="0.5em"
                mb="0.6em"
                src="~/assets/images/banner7.png"
              />
            </c-tab-panel>
            <c-tab-panel>
              <img
                v-chakra
                width="100%"
                pr="0.8em"
                border-radius="0.5em"
                mb="0.6em"
                src="~/assets/images/banner7.png"
              />
              <img
                v-chakra
                width="100%"
                pr="0.8em"
                border-radius="0.5em"
                mb="0.6em"
                src="~/assets/images/banner8.png"
              />
              <img
                v-chakra
                width="100%"
                pr="0.8em"
                border-radius="0.5em"
                mb="0.6em"
                src="~/assets/images/banner9.png"
              />
            </c-tab-panel>
            <c-tab-panel display="flex" justify-content="start">
              <img
                v-chakra
                width="100%"
                pr="0.8em"
                border-radius="0.5em"
                mb="0.6em"
                src="~/assets/images/banner10.png"
              />
            </c-tab-panel>
            <c-tab-panel>
              <img
                v-chakra
                width="100%"
                pr="0.8em"
                border-radius="0.5em"
                mb="0.6em"
                src="~/assets/images/banner9.png"
              />
              <img
                v-chakra
                width="100%"
                pr="0.8em"
                border-radius="0.5em"
                mb="0.6em"
                src="~/assets/images/banner8.png"
              />
            </c-tab-panel>
            <c-tab-panel>
              <img
                v-chakra
                width="100%"
                pr="0.8em"
                border-radius="0.5em"
                mb="0.6em"
                src="~/assets/images/banner10.png"
              />
            </c-tab-panel>
            <c-tab-panel>
              <img
                v-chakra
                width="100%"
                pr="0.8em"
                border-radius="0.5em"
                mb="0.6em"
                src="~/assets/images/banner7.png"
              />
            </c-tab-panel>
          </c-tab-panels>
        </c-grid-item>
      </c-grid>
    </c-tabs>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  data() {
    return {
      activeTab: 0,
    }
  },

  methods: {
    setActiveTab(index: number) {
      this.activeTab = index
    },
    pathForImage(filename: string) {
      return require(`~/assets/icons/${filename}`)
    },
  },
})
</script>
