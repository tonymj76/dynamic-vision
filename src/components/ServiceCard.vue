<template>
  <div>
    <div class="custom-row">
      <div class="custom-col" v-for="[title, body] in coreValue" :key="title">
        <h3 class="text-h4 core-h3 text-center text-md-left">
          {{ title }}
        </h3>
        <div>
          <p>
            {{ body }}
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ServiceCard",
  props: {
    coreValue: {
      type: Array,
      require: true,
    },
  },
};
</script>

<style scoped lang="scss">
.core-h3 {
  color: #456aa5;
}
.custom-row {
  display: flex;
  flex-flow: column;
  padding: 1px 0.5rem;
  .custom-col {
    width: 100%;
    padding-left: 10px;
    padding-top: 3rem;
    border-bottom: 1px solid rgba(171, 193, 217, 0.5);
  }
  .core-h3 {
    padding-bottom: 1rem;
  }
}
@media only screen and (min-width: 600px) {
  .custom-row {
    display: flex;
    flex-flow: row;
    .custom-col {
      width: 33.333%;
      border-left: 1px solid rgba(171, 193, 217, 0.5);
      border-bottom: none;
    }
    .custom-col:first-child {
      border-left: none;
      padding-left: 0;
    }
    .core-h3 {
      padding-bottom: 2rem;
    }
  }
}
</style>
