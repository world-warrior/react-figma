---
id: rectangle
title: Rectangle
---

Wrapper for the Figma [Rectangle](https://www.figma.com/plugin-docs/api/RectangleNode/).

#### Props

| Prop       | Type     | Default | Note                                              |
| ---------- | -------- | ------- | ------------------------------------------------- |
| `name`     | `String` |         | The name to be displayed in the Figma Layers List |
| `top` | `Number` |  |  |
| `left` | `Number` |  |  |
| `width` | `Number` |  |  |
| `height` | `Number` |  |  |
| `style`    | [`Style`](/docs/styling)   |  | Not all props |
| `onSelectionEnter` | `Function` |  | Selection enter event callback  |
| `onSelectionLeave` | `Function` |  | Selection leave event callback  |
| `onLayout` | `Function` |  | Event is fired once the layout has been calculated  |
| `onNodeId` | `Fuction` | | Getting Figma Node ID callback |  

Also, most of the [RectangleNode](https://www.figma.com/plugin-docs/api/RectangleNode/) fields are supported as props.

#### Example

```jsx
<Rectangle
    height={100}
    width={200}
/>
```
