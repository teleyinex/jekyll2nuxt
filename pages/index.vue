<template>
  <v-layout
    column
    justify-center
    align-center
  >
    <v-flex
      xs12
      sm8
      md6
    >
      <div class="text-xs-center" />
      <v-card>
        <v-card-title class="headline">
          Welcome to the Jekyll to Nuxt.js template
        </v-card-title>
        <v-card-text>
          <p>This is a <strong>basic</strong> template that you can modify to migrate your Jekyll site to a nuxtjs one.</p>
          <p>For importing your blogposts from Jekyll, all you have to do is the following:</p>
          <ol>
            <li>Copy all your blogposts from your jekyll site: _posts/ to content/blogposts.</li>
            <li>Run yarn dev</li>
          </ol>
          <p>
            That's it! By default the template comes with <nuxt-link to="/blog">
              two posts
            </nuxt-link>. One that has iframes and real code, while the other is only lorem ipsum ;-)
          </p>
          <p>As your front matter will be different, you might not see your cover images in the cards. Adapt it to your needs!</p>
          <p>
            The site uses Vuetify for the layout and components. For more information on Vuetify, check out the <a
              href="https://vuetifyjs.com"
              target="_blank"
            >
              documentation
            </a>.
          </p>
          <p>
            If you have questions, talk to me in Twitter<a
              href="https://twitter.com/teleyinex"
              target="_blank"
            >
              https://twitter.com/teleyinex 
            </a>.
          </p>
          <p>
            Find a bug? Report it on the github <a
              href="https://github.com/teleyinex/jekyll2nuxtjs/issues"
              target="_blank"
              title="contribute"
            >
              issue board
            </a>.
          </p>
          <p>Thank you for testing it.</p>
          <div class="text-xs-right">
            <em><small>&mdash; Daniel Lombraña</small></em>
          </div>
          <hr class="my-3">
          <a
            href="https://nuxtjs.org/"
            target="_blank"
          >
            Nuxt Documentation
          </a>
          <br>
          <a
            href="https://github.com/nuxt/nuxt.js"
            target="_blank"
          >
            Nuxt GitHub
          </a>
        </v-card-text>
        <v-card-actions>
          <v-btn
            color="primary"
            nuxt
            to="/blog"
          >
            Check the Blog
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-flex>
  </v-layout>
</template>

<script>
export default {}
</script>
