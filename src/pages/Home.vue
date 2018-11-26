<template>
    <div id="home" class="home">
        <Header />
        <Hero />
        <section class="section section-list">
            <div class="container">
                <h3 class="heading-secondary mb-medium text-center">Recent posts with <span class="text-italic">#resolution2019</span>..</h3>
                <Posts v-bind:postData="postData" />
            </div>
        </section>
        <section id="how-to" class="section section-how text-center">
            <div class="container">
                <h3 class="heading-secondary mb-small">You Can Get Involved Too. Here’s How..</h3>
                <Steps />
                <router-link to="/#" class="button">
                Share on Twitter
                </router-link>
            </div>
        </section>
        <CTASection />
        <Footer />
    </div>
</template>

<script>
import CTASection from '../components/cta-section'
import Footer from '../components/footer'
import Header from '../components/header'
import Hero from '../components/hero'
import dataForPosts from '../data/data.posts'
import Posts from '../components/posts'
import Steps from '../components/steps'
export default {
  name: 'Home',
  components: {
    CTASection,
    Footer,
    Header,
    Hero,
    Posts,
    Steps
  },
  data () {
    return {
      postData: [...dataForPosts]
    }
  }
}
</script>
