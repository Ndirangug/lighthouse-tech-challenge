<template>
  <c-grid
    id="info"
    align-items="center"
    :px="['0.8em', '2em', '4em', '10em']"
    template-columns="49% auto 49%"
    line-height="1em"
    mb="0.6em"
  >
    <c-grid-item pr="0.8em">
      <c-flex align="center">
        <c-flex>
          <img v-chakra width="7" height="6" src="~/assets/icons/ho_mo.png" />
        </c-flex>

        <c-flex ml="0.8em" direction="column">
          <p v-chakra color="brand.lightText" mb="0.4em">
            <span>KEN</span>
            <img v-chakra display="inline" src="~/assets/icons/ho_vi.png" />
            <span>7</span>
          </p>
          <p v-chakra color="brand.lightText" mb="0">
            $<span v-chakra font-size="1.1em" color="brand.gold"
              >122121233</span
            >
          </p>
        </c-flex>
      </c-flex>
    </c-grid-item>

    <c-grid-item>
      <div class="divider gradient-divider" />
    </c-grid-item>

    <c-grid-item px="0.8em">
      <div>
        <img
          v-chakra
          width="13px"
          display="inline"
          src="~/assets/icons/ho_no.png"
        />
        <c-text
          font-size="xs"
          color="brand.lightText"
          line-height="0"
          display="inline"
        >
          :Dragon Boat Festival. holiday! holiday! holiday! holiday! Dragon Boat
          Festival
        </c-text>
      </div>
    </c-grid-item>
  </c-grid>
</template>

<style scoped>
.gradient-divider {
  background: linear-gradient(black, white, black);
  height: 100%;
  width: 0.3em;
}
</style>
