<template>
  <q-cate-title
  :title="title"
  :show-line="showLine"
  />
  <div class="cate-list flex-box-space-wrap" :class="{ 'item-mb': showLine }">
    <q-cate-list-card />
    <q-cate-list-card />
    <q-cate-list-card />
    <q-cate-list-card />
    <q-cate-list-card />
    <q-cate-list-card />
  </div>
</template>
<script>
import QCateTitle from './QCateTitle.vue'
import QCateListCard from './QCateListCard.vue'
export default {
  components: { QCateTitle, QCateListCard },
  props: {
    title: {
      type: String,
      required: true
    },
    showLine: {
      type: Boolean,
      default: false
    }
  }
}
</script>
