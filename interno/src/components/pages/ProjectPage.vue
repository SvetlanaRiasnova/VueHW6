<template>
  <div class="project">
    <HeaderComponent />
    <section class="banner">
      <div class="banner__info">
        <h1 class="banner__info_header">Our Projects</h1>
        <div class="banner__info_breadcrump">Home / Project</div>
      </div>
    </section>
    <ProjectsCategoriesComponent @activCategories="activCategories" />
    <ProjectCardsComponent :projects="projects" />
    <div class="project__count_page">
      <div class="project__count_page-wrap">
        <a href="#" class="project__count_page-number">
          <p class="project__count_page-number-text">01</p>
        </a>
        <a href="#" class="project__count_page-number">
          <p class="project__count_page-number-text">02</p>
        </a>
        <a href="#" class="project__count_page-number">
          <p class="project__count_page-number-text">03</p>
        </a>
        <a href="#">
          <svg
            class="project__count_page-svg"
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
        </a>
      </div>
    </div>
    <FooterComponent />
  </div>
</template>

<script>
import HeaderComponent from "../HeaderComponent.vue";
import ProjectsCategoriesComponent from "../ProjectsPageCategoriesComponent.vue";
import ProjectCardsComponent from "../ProjectCardsComponent.vue";
import FooterComponent from "../FooterComponent.vue";
export default {
  name: "ProjectPage",
  components: {
    HeaderComponent,
    ProjectsCategoriesComponent,
    ProjectCardsComponent,
    FooterComponent,
  },
  data() {
    return {
      projects: [],
      projectsOne: [
        {
          id: 1,
          image: "project__img1.png",
          title: "Bathroom",
          text: "Decor / Artchitecture",
        },
        {
          id: 2,
          image: "project__img2.png",
          title: "Bathroom",
          text: "Decor / Artchitecture",
        },
        {
          id: 3,
          image: "project__img3.png",
          title: "Bathroom",
          text: "Decor / Artchitecture",
        },
        {
          id: 4,
          image: "project__img4.png",
          title: "Bathroom",
          text: "Decor / Artchitecture",
        },
        {
          id: 5,
          image: "project__img5.png",
          title: "Bathroom",
          text: "Decor / Artchitecture",
        },
        {
          id: 6,
          image: "project__img6.png",
          title: "Bathroom",
          text: "Decor / Artchitecture",
        },
        {
          id: 7,
          image: "project__img7.png",
          title: "Bathroom",
          text: "Decor / Artchitecture",
        },
        {
          id: 8,
          image: "project__img8.png",
          title: "Bathroom",
          text: "Decor / Artchitecture",
        },
      ],
      projectsTwo: [
        {
          id: 1,
          image: "project__img6.png",
          title: "Minimal Bedroom",
          text: "Decor / Artchitecture",
        },
        {
          id: 2,
          image: "project__img5.png",
          title: "Minimal Bedroom",
          text: "Decor / Artchitecture",
        },
        {
          id: 3,
          image: "project__img4.png",
          title: "Classic Minimal Bedroom",
          text: "Decor / Artchitecture",
        },
        {
          id: 4,
          image: "project__img3.png",
          title: "Modern Bedroom",
          text: "Decor / Artchitecture",
        },
        {
          id: 5,
          image: "project__img2.png",
          title: "Minimal Bedroom table",
          text: "Decor / Artchitecture",
        },
        {
          id: 6,
          image: "project__img1.png",
          title: "System Table",
          text: "Decor / Artchitecture",
        },
        {
          id: 7,
          image: "project__img7.png",
          title: "Modern Bedroom",
          text: "Decor / Artchitecture",
        },
        {
          id: 8,
          image: "project__img8.png",
          title: "Modern Bedroom",
          text: "Decor / Artchitecture",
        },
      ],
      projectsThree: [
        {
          id: 1,
          image: "project__img8.png",
          title: "Minimal Bedroom",
          text: "Decor / Artchitecture",
        },
        {
          id: 2,
          image: "project__img7.png",
          title: "Minimal Bedroom",
          text: "Decor / Artchitecture",
        },
        {
          id: 3,
          image: "project__img6.png",
          title: "Minimal Bedroom",
          text: "Decor / Artchitecture",
        },
        {
          id: 4,
          image: "project__img5.png",
          title: "Minimal Bedroom",
          text: "Decor / Artchitecture",
        },
        {
          id: 5,
          image: "project__img4.png",
          title: "Minimal Bedroom",
          text: "Decor / Artchitecture",
        },
        {
          id: 6,
          image: "project__img3.png",
          title: "Minimal Bedroom",
          text: "Decor / Artchitecture",
        },
        {
          id: 7,
          image: "project__img2.png",
          title: "Minimal Bedroom",
          text: "Decor / Artchitecture",
        },
        {
          id: 8,
          image: "project__img1.png",
          title: "Minimal Bedroom",
          text: "Decor / Artchitecture",
        },
      ],
      projectsFour: [
        {
          id: 1,
          image: "project__img4.png",
          title: "Minimal Bedroom",
          text: "Decor / Artchitecture",
        },
        {
          id: 2,
          image: "project__img5.png",
          title: "Minimal Bedroom",
          text: "Decor / Artchitecture",
        },
        {
          id: 3,
          image: "project__img3.png",
          title: "Minimal Bedroom",
          text: "Decor / Artchitecture",
        },
        {
          id: 4,
          image: "project__img2.png",
          title: "Minimal Bedroom",
          text: "Decor / Artchitecture",
        },
        {
          id: 5,
          image: "project__img1.png",
          title: "Minimal Bedroom",
          text: "Decor / Artchitecture",
        },
        {
          id: 6,
          image: "project__img6.png",
          title: "Minimal Bedroom",
          text: "Decor / Artchitecture",
        },
        {
          id: 7,
          image: "project__img7.png",
          title: "Minimal Bedroom",
          text: "Decor / Artchitecture",
        },
        {
          id: 8,
          image: "project__img8.png",
          title: "Minimal Bedroom",
          text: "Decor / Artchitecture",
        },
      ],
    };
  },

  created() {
    this.projects = this.projectsOne;
  },

  methods: {
    activCategories(data) {
      switch (data.id) {
        case 1:
          this.projects = this.projectsOne;
          break;
        case 2:
          this.projects = this.projectsTwo;
          break;
        case 3:
          this.projects = this.projectsThree;
          break;
        case 4:
          this.projects = this.projectsFour;
          break;
      }
    },
  },
};
</script>

<style lang="scss" scoped>
@import "../../style/variables.scss";
.banner {
  background-image: url("..//../assets/img/banner_product_page.png");
  min-height: 356px;
  @include flexCenter;
  align-items: flex-end;

  &__info {
    text-align: center;
    background-color: #fff;
    padding: 41px;
    border-radius: 37px 37px 0px 0px;

    &_header {
      // @include h2Style;
      text-align: left;
    }

    &_breadcrump {
      font-size: 22px;
      font-weight: 400;
      line-height: 33px;
    }
  }
}
// .project__categories {
//   margin-top: 200px;
//   display: flex;
//   justify-content: center;
//   flex-direction: column;
//   align-items: center;
//   &_wrap {
//     border-radius: 18px;
//     width: 880px;
//     border: 1px solid #cda274;
//     display: flex;
//     justify-content: space-evenly;
//     align-items: center;
//     gap: 63px;
//   }

//   &_button {
//     cursor: pointer;
//     padding: 26px 66px;
//     margin-left: -66px;
//     margin-right: -66px;

//     color: #292f36;
//     text-align: center;
//     // font-family: $familyText;
//     font-size: 18px;
//     font-style: normal;
//     font-weight: 600;
//     line-height: 125%;
//     letter-spacing: 0.36px;

//     &:hover {
//       color: #fff;
//       border-radius: 18px;
//       background: #cda274;
//     }
//   }
// }
// .active {
//   color: #fff;
//   border-radius: 18px;
//   background: #cda274;
// }
.project {
  &__count_page {
    margin-top: 51px;
    margin-bottom: 200px;
    display: flex;
    justify-content: center;

    &-wrap {
      display: flex;
      gap: 20px;
    }

    &-number {
      display: flex;
      justify-content: center;
      align-items: center;
      flex-wrap: nowrap;
      border: 1px #cda274 solid;
      width: 52px;
      height: 52px;
      border-radius: 52px;

      &-text {
        color: #292f36;
        font-family: $familyText;
        font-size: 16px;
        font-style: normal;
        font-weight: 500;
        line-height: 150%;
        text-transform: capitalize;
      }

      &:hover {
        background: #f4f0ec;
        border: none;
        width: 54px;
        height: 54px;
      }
    }

    &-svg:hover {
      fill: #f4f0ec;

      & circle {
        stroke: none;
      }
    }
  }
}
</style>
