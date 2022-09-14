<template>
  <c-flex p="2" class="title-bar" justify="space-between">
    <c-button variant="unstyled" aria-label="notifications">
      <img  src="~/assets/icons/ho_me.png" />
    </c-button>

    <img size="150px" src="~/assets/icons/ho_lo.png" />

    <c-menu>
      <c-menu-button variant="unstyled">
        <img  src="~/assets/icons/ho_li.png" />
      </c-menu-button>
      <c-menu-list minW="100px">
        <c-menu-item>Item1</c-menu-item>
        <c-menu-item>Item2</c-menu-item>
        <c-menu-item>Item3</c-menu-item>
        <c-menu-item>Item4</c-menu-item>
      </c-menu-list>
    </c-menu>
  </c-flex>
</template>
