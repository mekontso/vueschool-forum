<template>
  <div class="col-full">
    <h1>Welcome to the Forum</h1>
    <ForumList :forums="forums"/>
    <CategoryList :categories="categories"/>
  </div>
</template>

<script>
import sourceData from '@/data'
import ForumList from '@/components/ForumList'
import CategoryList from '@/components/CategoryList'
console.log(sourceData)
export default {
  components: {
    ForumList,
    CategoryList
  },
  data () {
    return {
      forums: Object.values(sourceData.forums),
      posts: sourceData.posts,
      users: sourceData.users,
      categories: Object.values(sourceData.categories)
    }
  }
}
</script>
