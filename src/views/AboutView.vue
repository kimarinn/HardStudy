<template>
<div>
  <div class="about">
    <h1>This is an about page</h1>
  </div>
  <div id="example-1">
    <input type="button" value="Test" onclick="alert('테스트')">
  </div>
  <div id="example-2">
    <button @click="counting">Count</button>
    <p>버튼을 클릭한 횟수: {{ counter }}</p>
  </div>
</div>
</template>
<script>
export default {
  name: 'example-2',
  data () {
    return {
      counter: 0
    }
  },
  methods: {
    counting () {
      this.counter++
    }
  }
}
</script>
