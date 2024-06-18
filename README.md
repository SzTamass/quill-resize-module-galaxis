# QUILL-RESIZE-MODULE

A module for Quill rich text editor to allow images to be resized.

## Usage

### Webpack/ES6

`npm install @galaxis/quill-resize-module`

```javascript
import Quill from "quill";
import ResizeModule from "@galaxis/quill-resize-module";

Quill.register("modules/resize", ResizeModule);

const quill = new Quill(editor, {
  modules: {
    resize: {
      locale: {
        altTip: "按住alt键比例缩放",
        inputTip: "回车键确认",
        floatLeft: "靠左",
        floatRight: "靠右",
        center: "居中",
        restore: "还原",
      },
    },
  },
});
```
