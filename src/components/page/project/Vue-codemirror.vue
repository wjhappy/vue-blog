<template>
  <div class="project">
    <codemirror v-model="code" :options="editorOption"></codemirror>
    <pre>{{ code }}</pre>
    <textarea v-model="code"></textarea>
  </div>
</template>

<script>
  export default {
    name: 'project-vue-codemirror',
    data() {
      return {
        code: 'const a = 10',
        editorOption: {
          tabSize: 4,
          mode: 'text/javascript',
          theme: 'base16-dark',
          lineNumbers: true,
          line: true,
          // ...
        }
      }
    }
  }
</script>
