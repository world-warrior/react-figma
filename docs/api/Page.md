---
id: page
title: Page
---

Wrapper for Figma [Pages](https://www.figma.com/plugin-docs/api/PageNode/).
Figma document (`figma.root`) should be a parent.


#### Props

| Prop       | Type     | Default | Note                                              |
| ---------- | -------- | ------- | ------------------------------------------------- |
| `name`     | `String` |         | The name to be displayed in the Figma Layers List |
| `children` | `Node`   |         |                                                   |
| `style`    | [`Style`](/docs/styling)   |         | Only layout props                                                 |
| `isCurrent`| `Boolean`|         | Make page current                                 |
| `onCurrentChange` | `Function` | | Changing current page callback |
| `backgrounds` | `Paint[]` | | Zero or one fill styles for the page |
| `onLayout` | `Function` |  | Event is fired once the layout has been calculated  |
| `onNodeId` | `Fuction` | | Getting Figma Node ID callback |  

#### Example

```jsx
<Page isCurrent name="My Page" style={{flexDirection: "row"}}>
  <Text>Hello world!</Text>
</Page>
```
