<template>
  <!--begin::Card-->
  <div class="card">
    <!--begin::Card Body-->
    <div class="card-body p-10 p-lg-15">
      <Overview></Overview>

      <BasicExamples></BasicExamples>
    </div>
    <!--end::Card Body-->
  </div>
  <!--end::Card-->
</template>

<script lang="ts">
import { defineComponent, onMounted } from "vue";
import { setCurrentPageTitle } from "@/core/helpers/breadcrumb";
import Overview from "@/views/resources/documentation/base/pagination/Overview.vue";
import BasicExamples from "@/views/resources/documentation/base/pagination/BasicExamples.vue";

export default defineComponent({
  name: "pagination",
  components: {
    Overview,
    BasicExamples
  },
  setup() {
    onMounted(() => {
      setCurrentPageTitle("Pagination");
    });
  }
});
</script>
