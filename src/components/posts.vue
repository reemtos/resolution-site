<template>
    <div class="posts">
        <div class="post" v-for="post in postData" v-bind:key="post.id">
            <div class="post__video-box">
            </div>
            <div class="post__details">
                <h4 class="heading-secondary username">@{{post.username}}</h4>
                <p class="paragraph small caption">{{post.resolution}}</p>
                <span class="date-posted">posted {{post.datePosted}}.</span>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'Posts',
  props: ['postData']
}
</script>
