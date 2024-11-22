# vue-validationcode-input

> 🎉A verification code input

## Install

```bash
npm install --save vue-validationcode-input
```

## Usage

```jsx
<template>
  <div id="app">
    <CodeInput :loading="false" class="input" v-on:change="onChange" v-on:complete="onComplete" />
  </div>
</template>

<script>
import CodeInput from "vue-validationcode-input";

export default {
  name: "app",
  components: {
    CodeInput
  },
  methods: {
    onChange(v) {
      console.log("onChange ", v);
    },
    onComplete(v) {
      console.log("onComplete ", v);
    }
  }
};
</script>
```

## PropTypes

|     Key     |  Type  |              Desc               |
| :---------: | :----: | :-----------------------------: |
|    type     |  text  |      one of number or text      |
|   fields    | number |     The count of characters     |
|  onChange   |  func  |   Trigger on character change   |
| onComplete  |  func  | Trigger on all character inputs |
| fieldWidth  | number |           input width           |
| fieldHeight | number |          input height           |
|  autoFocus  |  bool  | auto focus first input on init  |
|    title    | string |        code input title         |
|   loading   |  bool  |        show loading flag        |
|  className  | string |           class name            |
|   values    | array  |         default values          |

## License

MIT
