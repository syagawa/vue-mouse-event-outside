# v-outside-events

## usage

```html
<div id="app">
  <div><div>
  <div @class="click" v-outside-click="clickOutside">
    click me
  </div>
</div>
<script>
  import lib from "./index.js";

  new Vue({
    el: "#app",
    methods: {
      click: function(){
        console.log("click");
      },
      clickOutside: function(){
        console.log("click outside");
      }
    },
    directives: {
      "outside-click": {
        bind: lib.bind
      }
    }

  });

</script>

```
