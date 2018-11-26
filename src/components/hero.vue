<template>
    <section class="section section-hero">
        <div class="container">
            <div class="section-hero__grid">
                <div class="introduction">
                    <h1 class="heading-primary mb-small">Share your new year's resolutions with the world.</h1>
                    <h5 class="heading-tertiary mb-medium">From Instagram, to everybody.</h5>
                    <router-link to="/#how-to" class="button">
                    Show me how
                    </router-link>
                </div>
                <div class="illustration--box">
                    <img src="../assets/illustrations/hero.png" class="illustration" alt="hero illustration" />
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
  name: 'Hero'
}
</script>
