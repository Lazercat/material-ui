---
title: 扩展面板 React 组件
components: ExpansionPanel, ExpansionPanelActions, ExpansionPanelDetails, ExpansionPanelSummary
---
# 拓展面板

<p class="description">扩展面板包含创建流程，允许轻量编辑元素。</p>

[扩展面板](https://material.io/archive/guidelines/components/expansion-panels.html)是一个轻量级容器，既可以单独使用，也可以连接到更大的表面， 比如卡片。

## Simple Expansion Panel

{{"demo": "pages/demos/expansion-panels/SimpleExpansionPanel.js"}}

## Secondary heading and Columns

Multiple columns can be used to structure the content, and a helper text may be added to the panel to assist the user.

{{"demo": "pages/demos/expansion-panels/DetailedExpansionPanel.js"}}

## Controlled Accordion

Extend the default panel behavior to create an accordion with the `ExpansionPanel` component.

{{"demo": "pages/demos/expansion-panels/ControlledExpansionPanels.js"}}