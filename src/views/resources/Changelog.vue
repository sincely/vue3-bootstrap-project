<template>
  <!--begin::Card-->
  <div class="card">
    <!--begin::Card Body-->
    <div class="card-body p-10 p-lg-15">
      <!--begin::Accordion-->
      <div
        class="accordion accordion-flush accordion-icon-toggle"
        id="kt_accordion_2"
      >
        <!--begin::Item-->
        <div class="mb-5">
          <!--begin::Header-->
          <div
            class="accordion-header py-3 d-flex"
            data-bs-toggle="collapse"
            data-bs-target="#kt_accordion_2_item_1"
          >
            <span class="accordion-icon">
              <span class="svg-icon svg-icon-3">
                <inline-svg src="media/icons/duotone/Navigation/Right-2.svg" />
              </span>
            </span>
            <h3 class="fs-4 text-gray-800 fw-bold mb-0 ms-4">
              {{ themeName }} v8.0.11 - 26 May, 2021
            </h3>
          </div>
          <!--end::Header-->

          <!--begin::Body-->
          <div
            id="kt_accordion_2_item_2"
            class="fs-6 collapse show ps-10"
            data-bs-parent="#kt_accordion_2"
          >
            <h3 class="fs-6 fw-bolder mb-1">New:</h3>
            <ul class="py-2">
              <li class="py-2">
                Setup theme skeleton doc.
                <a
                  href="https://preview.keenthemes.com/metronic8/vue/demo1/#/documentation/setup-theme-skeleton"
                  >Preview</a
                >
              </li>
            </ul>
            <h3 class="fs-6 fw-bolder mb-1">Update:</h3>
            <ul class="py-2">
              <li class="py-2">
                Updated sign-in form buttons.
                <a
                  href="https://preview.keenthemes.com/metronic8/vue/demo1/#/sign-in"
                  >Preview</a
                >
              </li>
            </ul>
          </div>
          <!--end::Body-->
        </div>
        <!--end::Item-->

        <!--begin::Item-->
        <div class="mb-5">
          <!--begin::Header-->
          <div
            class="accordion-header py-3 d-flex"
            data-bs-toggle="collapse"
            data-bs-target="#kt_accordion_2_item_1"
          >
            <span class="accordion-icon">
              <span class="svg-icon svg-icon-3">
                <inline-svg src="media/icons/duotone/Navigation/Right-2.svg" />
              </span>
            </span>
            <h3 class="fs-4 text-gray-800 fw-bold mb-0 ms-4">
              {{ themeName }} v8.0.10 - 21 May, 2021
            </h3>
          </div>
          <!--end::Header-->

          <!--begin::Body-->
          <div
            id="kt_accordion_2_item_1"
            class="fs-6 collapse show ps-10"
            data-bs-parent="#kt_accordion_2"
          >
            <ul class="py-2">
              <li class="py-2">Initial release.</li>
            </ul>
          </div>
          <!--end::Body-->
        </div>
        <!--end::Item-->
      </div>
      <!--end::Accordion-->
    </div>
    <!--end::Card Body-->
  </div>
  <!--end::Card-->
</template>

<script lang="ts">
import { defineComponent, onMounted } from "vue";
import { themeName } from "@/core/helpers/documentation";
import { setCurrentPageTitle } from "@/core/helpers/breadcrumb";

export default defineComponent({
  name: "changelog",
  components: {},
  setup() {
    onMounted(() => {
      setCurrentPageTitle("Changelog");
    });

    return {
      themeName
    };
  }
});
</script>
