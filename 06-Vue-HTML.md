## Vue.js and HTML Attributes

- `v-on:input`
- `v-bild:class`
- Note: For `v-bind`, you may use `:class` instead of `v-bind:class`

```html
<div id="app">
  <input type="text" v-on:input="cssClass = $event.target.value" />
  <p v-bind:class="cssClass">Class: {{ cssClass }}</p>
  <!-- <p :class="cssClass">Class: {{ cssClass }}</p> -->
</div>
```

```css
.red {
  background-color: red;
}

.blue {
  background-color: blue;
  color: white;
}
```

```js
new Vue({
  el: "#app",
  data: {
    cssClass: ""
  }
});
```
