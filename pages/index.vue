<template>
  <div class="container">
    <div>
      <h1 class="title">
        ie11
      </h1>
      <code>Shift-ArrowLeft split</code>
      <ul>
        <li v-for="(part, index) in sal" :key="index"><code>{{part}}</code></li>
      </ul>
      <v-btn @click="split">Split Shift-ArrowLeft</v-btn>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      sal: []
    }
  },
  methods: {
    split() {
      this.sal = "Shift-ArrowLeft".split(/-(?!$)/);
    }
  }
}
</script>
