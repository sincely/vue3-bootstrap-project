<template>
  <div class="mb-10">
    <!--begin::Heading-->
    <h1 class="anchor fw-bolder mb-5">
      <a href="#tabs"></a>
      Tabs
    </h1>
    <!--end::Heading-->

    <!--begin::Block-->
    <div class="py-5">
      Divide data collections which are related yet belong to different types.
    </div>
    <!--end::Block-->
  </div>
  <EUIBasicUsage></EUIBasicUsage>
  <EUICardStyle></EUICardStyle>
  <EUIBorderCard></EUIBorderCard>
  <EUITabPosition></EUITabPosition>
  <EUICustomTab></EUICustomTab>
  <EUIAddAndCloseTab></EUIAddAndCloseTab>
  <EUICustomizedTriggerButtonOfNewTab></EUICustomizedTriggerButtonOfNewTab>
</template>

<script>
import { defineComponent } from "vue";
import { setCurrentPageTitle } from "@/core/helpers/breadcrumb";
import EUIBasicUsage from "@/views/resources/documentation/element-ui/navigation/tabs/BasicUsage.vue";
import EUICardStyle from "@/views/resources/documentation/element-ui/navigation/tabs/CardStyle.vue";
import EUIBorderCard from "@/views/resources/documentation/element-ui/navigation/tabs/BorderCard.vue";
import EUITabPosition from "@/views/resources/documentation/element-ui/navigation/tabs/TabPosition.vue";
import EUICustomTab from "@/views/resources/documentation/element-ui/navigation/tabs/CustomTab.vue";
import EUIAddAndCloseTab from "@/views/resources/documentation/element-ui/navigation/tabs/AddAndCloseTab.vue";
import EUICustomizedTriggerButtonOfNewTab from "@/views/resources/documentation/element-ui/navigation/tabs/CustomizedTriggerButtonOfNewTab.vue";

export default defineComponent({
  name: "tabs",
  components: {
    EUIBasicUsage,
    EUICardStyle,
    EUIBorderCard,
    EUITabPosition,
    EUICustomTab,
    EUIAddAndCloseTab,
    EUICustomizedTriggerButtonOfNewTab
  },
  setup() {
    setCurrentPageTitle("Tabs");
  }
});
</script>
