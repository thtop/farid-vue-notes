## Understanding Events and Methods in Vue.js

- `v-on:click`

```html
<div id="app">
  <button v-on:click="changeTitle">Change Title</button>
  <p>{{ title }}</p>
</div>
```

```js
new Vue({
  el: "#app",
  data: {
    title: "Hello World!"
  },
  methods: {
    changeTitle() {
      this.title = "Change Title";
    }
  }
});
```
