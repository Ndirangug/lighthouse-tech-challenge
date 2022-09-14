<template>
  <c-box py="0.8em" pl="0.8em">
    <p v-chakra color="brand.gold">Hot Games</p>

    <c-flex
      class="hot-games-banners"
      justify="start"
      align="center"
      overflow-x="scroll"
    >
      <c-image
        rounded="0.5em"
        object-fit="cover"
        mr="0.6em"
        size="20vw"
        :src="require(`~/assets/images/banner2.png`)"
      />
      <c-image
        rounded="0.5em"
        object-fit="cover"
        mr="0.6em"
        size="20vw"
        :src="require(`~/assets/images/banner3.png`)"
      />
      <c-image
        rounded="0.5em"
        object-fit="cover"
        mr="0.6em"
        size="20vw"
        :src="require(`~/assets/images/banner4.png`)"
      />
      <c-image
        rounded="0.5em"
        object-fit="cover"
        mr="0.6em"
        size="20vw"
        :src="require(`~/assets/images/banner5.png`)"
      />
      <c-image
        rounded="0.5em"
        object-fit="cover"
        mr="0.6em"
        size="20vw"
        :src="require(`~/assets/images/banner6.png`)"
      />
    </c-flex>
  </c-box>
</template>


<style scoped>
.hot-games-banners::-webkit-scrollbar {
  display: none;
}

.hot-games-banners {
  -ms-overflow-style: none;
  scrollbar-width: none;
}


</style>
