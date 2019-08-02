<template>
  <div>
    <nav class="bg-white px-8 ml-4 pt-2">
      <div class="flex justify-center">
        <a
          v-for="tab in tabs"
          :key="tab.name"
          class="no-underline uppercase font-bold text-xs py-3 px-5 rounded-t "
          :class="{
            'bg-red-700 text-white': tab.isActive,
            'bg-gray-100 text-red-700': tab.isActive == false
          }"
          :href="tab.href"
          @click="selectTab(tab)"
        >
          {{ tab.name }}
        </a>
      </div>
    </nav>

    <div class="tabs-details">
      <slot />
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return { tabs: [] }
  },
  created() {
    this.tabs = this.$children
  },
  methods: {
    selectTab(selectedTab) {
      this.tabs.forEach((tab) => {
        tab.isActive = tab.href == selectedTab.href
      })
    }
  }
}
</script>
