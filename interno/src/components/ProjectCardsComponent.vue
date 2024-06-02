<template>
  <div class="project__cards">
    <div
      class="project__cards_list"
      v-for="project in projects"
      :key="project.id"
    >
      <img
        class="project__item_img"
        :src="require('../assets/img/' + project.image)"
        alt="product image"
      />
      <div class="project__item_wrap">
        <div class="project__item_wrap-text">
          <h2 class="project__item_title">{{ project.title }}</h2>
          <p class="project__item_text">{{ project.text }}</p>
        </div>
        <div class="product__button">
          <button class="project__page_btn">
            <svg
              class="project__page-svg"
              xmlns="http://www.w3.org/2000/svg"
              width="53"
              height="52"
              viewBox="0 0 53 52"
              fill="none"
            >
              <circle cx="26.5" cy="26" r="25.5" stroke="#CDA274" />
              <path
                d="M23.5571 32L29.5 25.3143L23.5571 18.6286"
                stroke="#292F36"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ProjectCardsComponent",

  props: ["projects"],

  data() {
    return {};
  },
  methods: {},
};
</script>

<style lang="scss" scoped>
.project__cards {
  margin: 0 auto;
  padding-top: 60px;
  width: 1200px;
  display: grid;
  gap: 60px;
  grid-template-columns: repeat(2, auto);
  justify-content: center;
}
.project__items {
  margin-top: 61px;
  margin-bottom: 61px;
}

.project__item {
  padding-bottom: 27px;
  display: inline-block;

  &_wrap {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: nowrap;
    flex-direction: row;
  }
  .project__page_btn {
    background-color: inherit;
    border: none;
  }
  .project__page-svg:hover {
    fill: #f4f0ec;

    & circle {
      stroke: none;
    }
  }
}
</style>
