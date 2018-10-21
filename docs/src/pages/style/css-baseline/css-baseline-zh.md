---
components: CssBaseline
---
# CSS 基线

<p class="description">Material-UI 提供了一个 CssBaseline 组件, 用于启动一个优雅、一致且简单的基线。</p>

您可能熟悉 [normailize.css](https://github.com/necolas/normalize.css), 一个HTML 元素和属性样式规范化的集合。

```jsx
import React from 'react';
import CssBaseline from '@material-ui/core/CssBaseline';

function MyApp() {
  return (
    <React.Fragment>
      <CssBaseline />
      {/* The rest of your application */}
    </React.Fragment>
  );
}

export default MyApp;
```

## 方法

### 页面

`<html>` 和 `<body>` 元素将更新以提供更好的页面范围的默认设置。 更具体地说: -删除所有浏览器中的边距。 -默认使用Material Design的背景颜色。 它使用 [`theme.palette.background.default`](/customization/default-theme/?expend-path=$.palette.background) 在标准设备上而在打印设备上使用白色背景。

### 布局

- `box-sizing` 在 `<html>` 元素上全局设置为 `border-box`。 每个元素 包括 `*:: before` 和 `*:: after` 被声明去继承这个属性，它确保元素的声明宽度永远不会超过padding或者border。

### Typography

- 字体抗锯齿功能可以更好地显示Roboto字体
- No base font-size is declared on the `<html>`, but 16px is assumed (the browser default). You can learn more about the implications of changing the `<html>` default font size in [the theme documentation](/customization/themes/#typography-html-font-size) page.