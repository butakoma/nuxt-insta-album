<template>
  <div>
    <div v-for="post in posts" v-bind:key="post.userName">
      <div class="card">
        <div class="header">
          <div class="media">
            <div class="media-left">
              <figure class="image is-48x48">
                <img :src="post.profImage" alt="Placeholder image" />
              </figure>
            </div>
            <div class="media-content">
              <p class="title is-4">{{ post.userName }}</p>
              <p class="subtitle is-6">{{ post.userId }}</p>
            </div>
          </div>
        </div>
        <div class="card-image">
          <figure class="image is-4by3">
            <img :src="post.image" alt="Placeholder image" />
          </figure>
        </div>
        <div class="card-content">
          <div class="level is-mobile">
            <div class="level-left">
              <div class="level-item has-text-centered">
                <a href>
                  <i class="material-icons">favorite_border</i>
                </a>
              </div>
              <div class="level-item has-text-centered">
                <div>
                  <a href>
                    <i class="material-icons">chat_bubble_outline</i>
                  </a>
                </div>
              </div>
            </div>
          </div>

          <div class="content">
            <p>
              <strong>{{ post.likes }} Likes</strong>
            </p>
            {{ post.text }}
            <a>@bulmaio</a>.
            <a href="#">#css</a>
            <a href="#">#responsive</a>
            <br />
            <time>{{ post.datetime }}</time>
          </div>
        </div>
        <div class="card-footer">
          <div class="columns is-mobile">
            <div class="column is-11">
              <div class="field">
                <div class="control">
                  <input class="input is-medium" type="text" placeholder="Add a comment . . ." />
                </div>
              </div>
            </div>
            <div class="column has-text-centered">
              <button class="button">
                <i class="material-icons">more_horiz</i>
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import posts from '../pages/posts/post.json'

export default {
  data ({ params }) {
    return { posts }
  }
}
</script>
