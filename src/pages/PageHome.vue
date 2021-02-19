<template>
  <div class="col-full">
    <h1>Welcome to the Forum</h1>

    <CategoryList :categories="categories"/>
  </div>
</template>

<script>
import ForumList from '@/components/ForumList'
import CategoryList from '@/components/CategoryList'

export default {
  components: {
    ForumList,
    CategoryList
  },
  computed: {
    categories () {
      return Object.values(this.$store.state.categories)
    }
  },
  data () {
    return {

    }
  }
}
</script>
