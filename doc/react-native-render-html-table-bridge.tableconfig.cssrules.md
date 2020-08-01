<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [react-native-render-html-table-bridge](./react-native-render-html-table-bridge.md) &gt; [TableConfig](./react-native-render-html-table-bridge.tableconfig.md) &gt; [cssRules](./react-native-render-html-table-bridge.tableconfig.cssrules.md)

## TableConfig.cssRules property

Override default CSS rules with this prop.

<b>Signature:</b>

```typescript
cssRules?: string;
```

## Remarks

You should at least set a rule which adds a 0-margin to `body` and `html`<!-- -->, otherwise the table will look truncated. When set, `tableStyleSpecs` is ignored. If you want to extend default instead of override CSS styles, look at example bellow.

## Example


```
const cssRules = cssRulesFromSpecs(defaultTableStylesSpecs) + `
a {
  text-transform: uppercase;
}
`;

const config = {
  cssRules,
  // Other config options
};

```
