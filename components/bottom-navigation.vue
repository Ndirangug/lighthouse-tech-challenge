<template>
  <c-box
    v-chakra
    position="fixed"
    bottom="1.2em"
    left="50%"
    background="#303032"
    border-radius="0.8em"
    transform="translateX(-50%)"
    mx="auto"
    width="80vw"
    justify-content="space-around"
    display="flex"
    align-items="center"
    class="bottom-navigation"
    box-shadow="lg"
    py="1em"
    px="1em"
  >
    <c-button variant="unstyled" @click="navigate(0, '/')">
      <tab-switcher
        v-chakra
        height="100%"
        :active-image="pathForImage('ho_ho1@3x.png')"
        :inactive-image="pathForImage('ho_ho2@3x.png')"
        :index="0"
        :active-tab="activeTab"
      />
    </c-button>

    <c-button variant="unstyled" @click="navigate(1, '/activity')">
      <tab-switcher
        v-chakra
        height="100%"
        :active-image="pathForImage('ho_ac1@3x.png')"
        :inactive-image="pathForImage('ho_ac2@3x.png')"
        :index="1"
        :active-tab="activeTab"
      />
    </c-button>

    <c-button variant="unstyled" @click="navigate(2, '/wallet')">
      <tab-switcher
        v-chakra
        height="100%"
        :active-image="pathForImage('ho_wa1@3x.png')"
        :inactive-image="pathForImage('ho_wa2@3x.png')"
        :index="2"
        :active-tab="activeTab"
      />
    </c-button>

    <c-button variant="unstyled" @click="navigate(3, '/live-chat')">
      <tab-switcher
        v-chakra
        height="100%"
        :active-image="pathForImage('ho_co1@3x.png')"
        :inactive-image="pathForImage('ho_co2@3x.png')"
        :index="3"
        :active-tab="activeTab"
      />
    </c-button>

    <c-button variant="unstyled" @click="navigate(4, '/my-account')">
      <tab-switcher
        v-chakra
        height="100%"
        :active-image="pathForImage('ho_my1@3x.png')"
        :inactive-image="pathForImage('ho_my2@3x.png')"
        :index="4"
        :active-tab="activeTab"
      />
    </c-button>
  </c-box>
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
    pathForImage(filename: string) {
      return require(`~/assets/icons/${filename}`)
    },
    navigate(index: number, path: string) {
      this.activeTab = index
      this.$router.push(path)
    },
  },
})
</script>
