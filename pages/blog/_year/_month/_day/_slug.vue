<template lang="pug">
v-container(fluid grid-list-xl)
  v-layout(row wrap)
    v-flex(xs12, md6)
        v-img(:src='blog.photo_url', :aspect-ratio='4/3')
        .blogContent(v-html="$md.render(blog.content)")
</template>
<script>
export default {
  async asyncData({ app, params }) {
    const slug = `${params.year}-${params.month}-${params.day}-${params.slug}`
    const blogposts = await app.$axios.$get('/blogposts.json')
    const blog = blogposts[slug]

    blog.content = blog.content.replace('<!--more-->', '')

    return {
      blog
    }
  }
}
</script>
<style lang="scss">
code {
  display: flex;
  padding: 15px;
  margin-bottom: 64px;
  overflow: scroll;
}
.blogContent > p > img {
  display: block;
  max-width: 100%;
  height: auto;
}
</style>
