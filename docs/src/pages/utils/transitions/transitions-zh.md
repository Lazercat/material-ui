---
title: Transition React component
components: Collapse, Fade, Grow, Slide, Zoom
---
# Transitions

<p class="description">过渡有助于使UI富有表现力且易于使用。</p>

Material-UI提供了一系列过渡效果, 使一些 [动作](https://material.io/design/motion/) 可以被添加到你的组件中.

为了更好地支持服务端渲染, Material-UI 为某些过渡组件 (Fade, Grow, Zoom, Slide) 的子级提供了 `style` 属性 。 为了使动画按预期实现, 必须添加`style`属性到DOM上.

```jsx
// The `props` object contains a `style` property.
// You need to provide it to the `div` element as shown here.
function MyComponent(props) {
  return (
    <div {...props}>
      Fade
    </div>
  );
}

export default Main() {
  return (
    <Fade>
      <MyComponent />
    </Fade>
  );
}
```

## Collapse

Expand vertically from the top of the child element. The `collapsedHeight` property can be used to set the minimum height when not expanded.

{{"demo": "pages/utils/transitions/SimpleCollapse.js"}}

## Fade

Fade in from transparent to opaque.

{{"demo": "pages/utils/transitions/SimpleFade.js"}}

## Grow

Expand outwards from the center of the child element, while also fading in from transparent to opaque.

The second example demonstrates how to change the `transform-origin`, and conditionally applies the `timeout` property to change the entry speed.

{{"demo": "pages/utils/transitions/SimpleGrow.js"}}

## Slide

Slide in from the edge of the screen. The `direction` property controls which edge of the screen the transition starts from.

The Transition component's `mountOnEnter` property prevents the child component from being mounted until `in` is `true`. This prevents the relatively positioned component from scrolling into view from it's off-screen position. Similarly the `unmountOnExit` property removes the component from the DOM after it has been transition off screen.

{{"demo": "pages/utils/transitions/SimpleSlide.js"}}

## 放大

从子元素的中心向外扩展。

此示例还演示如何延迟输入过渡。

{{"demo": "pages/utils/transitions/SimpleZoom.js"}}