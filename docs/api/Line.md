---
id: line
title: Line
---

Wrapper for the Figma [Line](https://www.figma.com/plugin-docs/api/LineNode/).

#### Props

| Prop       | Type     | Default | Note                                              |
| ---------- | -------- | ------- | ------------------------------------------------- |
| `name`     | `String` |         | The name to be displayed in the Figma Layers List |
| `strokeWeight` | `Number` |         |  |
| `strokes` | Array of [Paint](https://www.figma.com/plugin-docs/api/Paint/) |         |  |
| `style`    | [`Style`](/docs/styling)   |         | Not all props                                                 |
| `onSelectionEnter` | `Function` |  | Selection enter event callback  |
| `onSelectionLeave` | `Function` |  | Selection leave event callback  |
| `onLayout` | `Function` |  | Event is fired once the layout has been calculated  |
| `onNodeId` | `Fuction` | | Getting Figma Node ID callback |  

Also, most of the [LineNode](https://www.figma.com/plugin-docs/api/LineNode/) fields are supported as props.

#### Example

```jsx
<Line
    name="line"
    strokeWeight={4}
    strokeAlign="CENTER"
    opacity={0.5}
    strokes={[{ type: 'SOLID', color: { r: 1, g: 0, b: 1 } }]}
    strokeCap="ROUND"
    dashPattern={[2, 10, 2, 10]}
/>
```
