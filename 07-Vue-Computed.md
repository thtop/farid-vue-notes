## Vue.js and Computed Properties

```html
<div id="app">
  <button v-on:click="increment">Increment</button>
  <p>Counter: {{ counter }}</p>
  <p>Clicks: {{ clicks }}</p>
</div>
```

```js
new Vue({
  el: "#app",
  data: {
    counter: 0,
    clicks: 0
  },
  methods: {
    increment() {
      /* 	this.counter = this.clicks * 2; */
      this.clicks++;
    }
  },
  computed: {
    counter() {
      return this.clicks * 2;
    }
  }
});
```
