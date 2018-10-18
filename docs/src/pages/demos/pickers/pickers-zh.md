---
title: Date Picker, Time Picker React component
components: TextField
---
# 选择器

<p class="description">选择器提供了一种从预先设定的集合中选取单个值的简单方法。</p>

- 在移动端，选择器最适合在确认对话框中展示。
- 对于内联显示（如在一个表单中），请考虑使用紧凑型控件，如分段下拉按钮。

#### 注意

We are currently falling back to **native input controls**. If you are interested in implementing or have implemented a rich Material Design Picker with an awesome UX, please, let us know on [#4787](https://github.com/mui-org/material-ui/issues/4787) and [#4796](https://github.com/mui-org/material-ui/issues/4796)! We could add a link to or a demo of your project in the documentation. Here are some components that are **promising**: - [material-ui-pickers](https://github.com/dmtrKovalenko/material-ui-pickers): date pickers and time pickers. - [material-ui-time-picker](https://github.com/TeamWertarbyte/material-ui-time-picker): time pickers. - [material-ui-next-pickers](https://github.com/chingyawhao/material-ui-next-pickers): date pickers and time pickers.

⚠️ Native input controls support by browsers [isn't perfect](https://caniuse.com/#feat=input-datetime).

## 日期选择器

一个原生日期选择器示例 `type="date"`，它也可以用作日历：

{{"demo": "pages/demos/pickers/DatePickers.js"}}

## Time pickers

A native time picker example with `type="time"`:

{{"demo": "pages/demos/pickers/TimePickers.js"}}

## Date & Time pickers

A native date & time picker example with `type="datetime-local"`:

{{"demo": "pages/demos/pickers/DateAndTimePickers.js"}}